# Overview

The Legerity framework for speeding up development with .NET & Appium is seprated into multiple areas covering:

- [Page Object Pattern (POP)](../src/Legerity/Pages/BasePage.cs)
  - The goal of the page object pattern is to use page objects to abstract page information away from your tests. Ideally, they will store all your selectors to find UI elements that a page is aware of and actions that are capable of the page. 

- Platform control wrappers
  - The goal of the platform control wrappers is to provide an easy set of elements which surface up properties and actions of the actual controls within the UI to make it easier for you to write tests that interact with them. 

## Page Object Pattern (POP)

The page object pattern has been implemented in a very simple and easy way to start utilizing in your own test projects. 

The Windows Alarms And Clock sample project provides an easy to understand example of how to implement a page within your tests in the form of the [EditAlarmPage](../samples/WindowsAlarmsAndClock/Pages/EditAlarmPage.cs).

[Read more about implementing POP](POP.md).

## Platform control wrappers

Platform control wrappers are as simple as they sound. They are a wrapper around the Appium element (AppiumWebElement, WindowsElement, AndroidElement etc.) which provide better actions for interaction and exposed properties to give you an easier development experience with UI tests. 

Currently the project supports the core UWP interactive controls with plan to expand to core iOS and Android controls in Xamarin.

These are built in a way that also allows you to extend the base wrapper to create wrappers for your own custom controls! 

[Read more about using control wrappers](ControlWrappers.md)