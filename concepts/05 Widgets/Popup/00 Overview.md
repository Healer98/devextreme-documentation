The **Popup** widget is a pop-up window overlaying the current view. 

<a href="https://js.devexpress.com/Demos/WidgetsGallery/#demo/dialogs_and_notifications-popup-overview" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>

The following code adds a simple **Popup** to your page, along with a [Button](/concepts/05%20Widgets/Button/00%20Overview.md '/Documentation/Guide/Widgets/Button/Overview/') that invokes it. The simplest configuration of the **Popup** requires the content and [title](/api-reference/10%20UI%20Widgets/dxPopup/1%20Configuration/title.md '/Documentation/ApiReference/UI_Widgets/dxPopup/Configuration/#title') to be specified. 

    <!--HTML-->
    <div id="popupContainer">
        <p>Popup content</p>
    </div>
    <div id="buttonContainer"></div>

<!---->

    <!--JavaScript-->
    $(function() {
        $("#popupContainer").dxPopup({
            title: "Popup Title"
        });
                
        $("#buttonContainer").dxButton({
            text: "Show the Popup", 
            onClick: function () {
                $("#popupContainer").dxPopup("show");
            } 
        });
    });

There are several ways to specify the content of the **Popup**. Learn more in the [Customize the Content](/concepts/05%20Widgets/Popup/05%20Customize%20the%20Appearance/05%20Customize%20the%20Content.md '/Documentation/Guide/Widgets/Popup/Customize_the_Appearance/Customize_the_Content/') article. The **Popup** can also be displayed with a toolbar. For detailed information, see the [Specify Toolbar Items](/concepts/05%20Widgets/Popup/05%20Customize%20the%20Appearance/20%20Specify%20Toolbar%20Items.md '/Documentation/Guide/Widgets/Popup/Customize_the_Appearance/Specify_Toolbar_Items/') topic. 

#####See Also#####
- [Widget Basics - jQuery](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/')
- [Widget Basics - AngularJS](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/')
- [Widget Basics - Knockout](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/')
- [Popup - Customize the Appearance](/concepts/05%20Widgets/Popup/05%20Customize%20the%20Appearance/05%20Customize%20the%20Content.md '/Documentation/Guide/Widgets/Popup/Customize_the_Appearance/Customize_the_Content/')
- [Popup - Show and Hide the Popup](/concepts/05%20Widgets/Popup/10%20Show%20and%20Hide%20the%20Popup '/Documentation/Guide/Widgets/Popup/Show_and_Hide_the_Popup/')
- [Popup - Resize and Relocate](/concepts/05%20Widgets/Popup/15%20Resize%20and%20Relocate.md '/Documentation/Guide/Widgets/Popup/Resize_and_Relocate/')
- [Popup API Reference](/api-reference/10%20UI%20Widgets/dxPopup '/Documentation/ApiReference/UI_Widgets/dxPopup/')

[tags]popup, overview, overlay