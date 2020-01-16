You can delete **List** items programmatically in the following ways.

- **By index**        
Pass the index to the [deleteItem(itemIndex)](/api-reference/10%20UI%20Widgets/dxList/3%20Methods/deleteItem(itemIndex).md '/Documentation/ApiReference/UI_Widgets/dxList/Methods/#deleteItemitemIndex') method. If the **List** is [grouped](/concepts/05%20Widgets/List/14%20Grouping/01%20In%20the%20Data%20Source.md '/Documentation/Guide/Widgets/List/Grouping/In_the_Data_Source/'), this method should be given an object with the indexes of the group and the item to be deleted.

        <!--JavaScript-->
        var list = $("#listContainer").dxList("instance");
        // Deletes the item with index 1 
        list.deleteItem(1);
        // Deletes the item with index 0 from the group with index 2
        list.deleteItem({ group: 2, item: 0 });

- **By DOM node**      
Pass the [DOM node](https://www.w3schools.com/js/js_htmldom_nodes.asp) to the [deleteItem(itemElement)](/api-reference/10%20UI%20Widgets/dxList/3%20Methods/deleteItem(itemElement).md '/Documentation/ApiReference/UI_Widgets/dxList/Methods/#deleteItemitemElement') method.

        <!--JavaScript-->
        var list = $("#listContainer").dxList("instance");
        // Finds all List items
        var itemNodes = $("#listContainer").find(".dx-list-item");
        // Makes the first item the last
        list.deleteItem(itemNodes[itemNodes.length-1]);

[note]If you want to delete an item by key or by data object, do it directly in the data source.

#####See Also#####
- [Widget Basics - Call Methods](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery/10%20Call%20Methods.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/Call_Methods/')
- [List Demos](https://js.devexpress.com/Demos/WidgetsGallery/Demo/List/ListSelection/jQuery/Light)
- [List API Reference](/api-reference/10%20UI%20Widgets/dxList '/Documentation/ApiReference/UI_Widgets/dxList/')
