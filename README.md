# NavigationDrawerMenuInfo

Creates a way to gather the selected index of menu items in a Navigation attached menu

Constructor- receieves a NavigationView Object, gets the map attached the the view and creates a Collections<List> of all item Ids in the Menu. Since there is no way to find out how many item are in the Menu the While loop  runs until the IndexOutOfBounds Exception is thrown.

<b>Finding the Index Of Menu Item Selected</b>
In the Overriden method onNavigationItemSelected() call findIndexOfMenuItem(MenuItem menuItem); or findIndexOfMenuItem(int itemId);
will return the index of the MenuItem selected in the menu

Good for interfaces that interact with TabLayouts,ViewPagers,ScrollViews,Fragments to handle multiple navigations in an Activity
