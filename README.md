Class to handle caching data about users from an SQL database when they join

Example usage:

//Input Database login info and the variables that you want to cache when a player joins
//Format is table.variable
cache = new Cache(this, "*ip*", "*port*", "*database*", "*username*", "*password*", "kitpvp.level", "kitpvp.archer", "kitpvp.warrior", "skywars.scout", "skywars.wizard", "skywars.farmer");

//add each database, listing all of the variables in the database, even those not cached
cache.addDatabase("kitpvp", new String[]{"level", "archer", "warrior", "kills"});
cache.addDatabase("skywars", new String[]{"scout", "wizard", "farmer", "kills"});

//get a variable
cache.get("table.variable", event.getPlayer())
cache.get("kitpvp.level", event.getPlayer())

//set a variable
cache.put("kitpvp.level", event.getPlayer())




