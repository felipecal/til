<h1>Associations in Sequelize</h1>

It is important to first define inside of the models the associations
that we will have between the tables and if there is to be a field as in the example below that is specified.

<h2>One to One</h2>

```
    Foo.hasOne(Bar);
    Bar.belongsTo(Foo, {
      foreignKey: 'myFooId'
    });
```

<h2>One to Many</h2>

Example with 2 tables User and Models

<p align="center">Models-Post</p>
It is important to define in the fields which attributes will be related to each other

```    author: {
      type: DataTypes.STRING,
      allowNull: false,
      references: {
        model: 'user',
        key: 'first_name'
      }
```
At the end of the models we have to define the relationships between the tables.

```
Post.associate = (models) => {
    Post.belongsTo(models.user, {
      foreignKey: 'id'
    })
```

<p align="center">Models-User</p>

```    User.associate = (models) => {
        User.hasMany(models.post, {
            foreignKey: 'id'
        })
```
