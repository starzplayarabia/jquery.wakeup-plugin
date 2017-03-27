jquery.wakeup-plugin
====================

An AMD wrapper of the JQuery plugin that will help detecting waking up from sleep and/or hibernation and executing assigned functions. This will allow us using this with RequireJS

Based on code provided by Andrew Mu: http://stackoverflow.com/questions/4079115


Usage
=====

```
// assign a handler function to be executed after waking up
var bell_id = $.wakeUp(function(sleep_time) {
    alert("I have slept for " + sleep_time/1000 + " seconds")
});

// remove this handler
$.ignoreBell(bell_id);

// remove all handlers
$.dreamOn();

```
