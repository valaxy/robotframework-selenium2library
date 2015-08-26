This is fork of `robotframework-selenium2library <https://github.com/rtomac/robotframework-selenium2library>`_

Currently robotframework-selenium2library version: 1.7.3

Main Work
=========
Add a keyword **use appium webdriver** which is exactly same with **create webdriver**,
instead of creating a new webdriver but use a opened appium webdriver

The library is aim at working together with `robotframework-appiumlibrary <https://github.com/valaxy/robotframework-appiumlibrary>`_

Usage
=====
::robotframework

    *** Settings ***
    library           AppiumLibrary
    library           Selenium2Library

    *** Test Cases ***
    test
        set library search order    AppiumLibrary    Selenium2Library
        open application2    ...
        use appium webdriver