//-------------------------
// Single Page Apps with HTML5, ASP.NET Web API, Knockout and jQuery
//
// Pluralsight
// John Papa
// http://twitter.com/john_papa
// Course: http://jpapa.me/spaps
// 
// Requirements to run the CodeCamper examples
//
// Live demo: http://jpapa.me/codecamperdemo
//-------------------------

// Notes
//-------------------------
spa-(m2|m3|m4)-xxx.zip contain the code for the demos shown in modules 2-4 of the course.

CodeCamper.zip contains the entire Code Camper application as shown in modules 5-11 of the course.

// Tools
//-------------------------
Visual Studio 2012

// Browser
//-------------------------
Recommended: Chrome, FireFox, Safari, or IE 9 

Debugging:
If using Safari, be sure to enable deugging tools
If using FireFox, be sure to isntall FireBug


// Extensions and Upates
//-------------------------
NuGet Package Manager
Web Essentials 2012 (supports LESS editing and CSS helpers)


// NuGet Packages (server)
//-------------------------
dotless >= 1.3.0.5
EntityFramework >= 5.0.0
Json.NET >= 4.5.8 
Microsoft ASP.NET MVC 4
Microsoft ASP.NET Web API
Microsoft ASP.NET Web Optimization Framework
Ninject >= 3.0.1.10


// NuGet Packages (client)
//-------------------------
jQuery >= 1.7.2
JSON-js json2 (for <= IE 7)
KnockoutJS >= 2.1.0
Knockout.js External Template Engine >= 2.0.5
    (also installs infuser and TrafficCop)
KoLite >= 1.0.3
Modernizr >= 2.0.20710
Moment.js >= 1.6.2
RequireJS >= 2.0.4.1
Sammy >= 0.6.3
toastr >= 1.0.2
underscore.js >= 1.3.3



// Optional Tools 
//-------------------------
Electric Mobile Studio 2012 http://www.electricplum.com/studio.aspx
http://jsfiddle.net
http://responsinator.com/



// Tips for Creating a SPA in Visual Studio 
//-------------------------
Create a "New MVC - Web API Project" 

Add NuGet Packages listed above

In Web.config set
<add key="webpages:Enabled" value="true" />

- Set this, otherwise we get "An ASP.NET setting has been detected that does not apply in Integrated managed pipeline mode"
<validation validateIntegratedModeConfiguration="false"/>

- Set this, otherwise you may get a 404 error for PUT and DELETE requests
<system.webServer>
    <validation validateIntegratedModeConfiguration="false" />
    <modules runAllManagedModulesForAllRequests="true" />
</system.webServer>


LESS
- Set cache to false. Otherwise errors don’t always show up. Be sure to turn caching on again later, to get performance.

<dotless minifyCss="false" cache="false" web="false" />



