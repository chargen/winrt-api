---
-api-id: T:Windows.UI.Xaml.Automation.Peers.SearchBoxAutomationPeer
-api-type: winrt class
---

<!-- Class syntax.
public class SearchBoxAutomationPeer : Windows.UI.Xaml.Automation.Peers.FrameworkElementAutomationPeer, Windows.UI.Xaml.Automation.Peers.ISearchBoxAutomationPeer
-->

# Windows.UI.Xaml.Automation.Peers.SearchBoxAutomationPeer

## -description
Exposes [SearchBox](../windows.ui.xaml.controls/searchbox.md) types to Microsoft UI Automation.

## -remarks
The Windows Runtime  [SearchBox](../windows.ui.xaml.controls/searchbox.md) class creates a new [SearchBoxAutomationPeer](searchboxautomationpeer.md) as its [OnCreateAutomationPeer](../windows.ui.xaml/uielement_oncreateautomationpeer_1478162674.md) definition. Derive your automation peer from [SearchBoxAutomationPeer](searchboxautomationpeer.md) if you are deriving a custom class from [SearchBox](../windows.ui.xaml.controls/searchbox.md) and want to add automation support for additional features that you enabled in your custom class. Then override [OnCreateAutomationPeer](../windows.ui.xaml/uielement_oncreateautomationpeer_1478162674.md) so that it returns your custom peer.

### Default peer implementation and overrides in **SearchBoxAutomationPeer**

[SearchBoxAutomationPeer](searchboxautomationpeer.md) has overrides of **Core** methods such that the associated [AutomationPeer](automationpeer.md) methods provide peer-specific information to a Microsoft UI Automation client.

+ [GetPattern](automationpeer_getpattern.md) reports no pattern support
+ [GetClassName](automationpeer_getclassname.md) returns "SearchBox".
+ [GetAutomationControlType](automationpeer_getautomationcontroltype.md) returns [AutomationControlType.Group](automationcontroltype.md).
The peer also has other behaviors that are provided by the base [FrameworkElementAutomationPeer](frameworkelementautomationpeer.md) class. For more info, see "Base implementation in FrameworkElementAutomationPeer" section of [Custom automation peers](http://msdn.microsoft.com/library/aa8da53b-fe6e-40ac-9f0a-cb09637c87b4).

## -examples

## -see-also
[FrameworkElementAutomationPeer](frameworkelementautomationpeer.md)