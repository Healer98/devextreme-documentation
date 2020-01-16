When the **LoadPanel** is shown, the area beneath it can be shaded. The shading color is specified by the [shadingColor](/api-reference/10%20UI%20Widgets/dxLoadPanel/1%20Configuration/shadingColor.md '/Documentation/ApiReference/UI_Widgets/dxLoadPanel/Configuration/#shadingColor') option.

    <!--JavaScript-->$(function() {
		$("#loadPanelContainer").dxLoadPanel({
            closeOnOutsideClick: true,
            shadingColor: "rgba(0, 0, 0, 0.2)"
        });
        
        $("#buttonContainer").dxButton({
            text: "Show the Load Panel", 
            onClick: function () {
                $("#loadPanelContainer").dxLoadPanel("show");
            } 
        });
    });

#####See Also#####
- [LoadPanel - Customize the Loading Indicator](/concepts/05%20Widgets/LoadPanel/10%20Customize%20the%20Appearance/10%20Customize%20the%20Loading%20Indicator.md '/Documentation/Guide/Widgets/LoadPanel/Customize_the_Appearance/Customize_the_Loading_Indicator/')
- [LoadPanel - Change the Text](/concepts/05%20Widgets/LoadPanel/10%20Customize%20the%20Appearance/20%20Change%20the%20Text.md '/Documentation/Guide/Widgets/LoadPanel/Customize_the_Appearance/Change_the_Text/')
- [LoadPanel - Hide the Pane](/concepts/05%20Widgets/LoadPanel/10%20Customize%20the%20Appearance/30%20Hide%20the%20Pane.md '/Documentation/Guide/Widgets/LoadPanel/Customize_the_Appearance/Hide_the_Pane/')
- [LoadPanel - Resize and Relocate](/concepts/05%20Widgets/LoadPanel/15%20Resize%20and%20Relocate.md '/Documentation/Guide/Widgets/LoadPanel/Resize_and_Relocate/')
- [LoadPanel Demos](https://js.devexpress.com/Demos/WidgetsGallery/#demo/dialogs_and_notifications-load_panel-overview)
- [LoadPanel API Reference](/api-reference/10%20UI%20Widgets/dxLoadPanel '/Documentation/ApiReference/UI_Widgets/dxLoadPanel/')

[tags]loadPanel, load panel, overlay, load panel shading, background, shading color