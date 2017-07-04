# Fancybox for Joomla

## UNMAINTAINED PROJECT
This project is no longer maintained. Any issues will not be actively picked up. Pull Requests will be merged unchecked. The sources here are up-for-grabs.

## Introduction
Font Awesome offers a great way to add HTML icons to your Joomla site. With this plugin, you can easily add the Font Awesome source to your site. But there's more: Instead of typing in the required fa code - which can cost you a lot of time, and which is not visible in the WYSIWYG environment of your backend - you can use Font Awesome tags to get your icons in there even quicker.

## Usage
First of all, the plugin simply loads the FontAwesome library remotely. Second, any FontAwesome tag in your content will be translated into an icon:

    {fa fa-camera-retro fa-2x}
    {fa fa-spinner fa-spin}
    {fa fa-circle-o-notch fa-spin}

The arguments after `{fa ...}` can include the `fa-` prefix, or the prefix can be skipped.

    {(fa fa-book}
    {(fa book}
    {fa fa-book}

Stacking is done by adding brackets:

    {fa fa-stack fa-lg [fa-square-o fa-stack-2x][fa-twitter fa-stack-1x]}
    
To make it easier to use the same sequence multiple times, you can add the following to the plugins alias box:

    stuff="fa-stack fa-lg [fa-square-o fa-stack-2x][fa-twitter fa-stack-1x]"

Or shorter:

    stuff="stack lg [square-o stack-2x][twitter stack-1x]"

And now the following will do as well:

    {fa stuff}
