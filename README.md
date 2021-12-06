### Built with

-HTML, CSS, Javascript, ejs, node.js, mongoDB, mongoose, express, 



### What I learned

- render database items in the todolist

- adding new items

- delete items from database 

- create custom lists using express route parameters 

EXAMPLE CODE:
```
  app.get("/:customListName", function(req, res){
  const customListName = _.capitalize(req.params.customListName);

  List.findOne({name: customListName}, function(err, foundList){
  if (!err){
    if (!foundList){
      //create a new list
      const list = new List({
        name: customListName,
        items: defaultItems
      });
```

- add new items to custom todo lists 

- delete items from custom todo lists

#LIVE SITE 
https://guarded-wildwood-23995.herokuapp.com/

