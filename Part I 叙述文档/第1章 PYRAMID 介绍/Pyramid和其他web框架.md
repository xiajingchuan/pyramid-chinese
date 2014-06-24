The first release of Pyramid’s predecessor (named repoze.bfg) was made in July of 2008. At the end
of 2010, we changed the name of repoze.bfg to Pyramid. It was merged into the Pylons project as
Pyramid in November of that year.
Pyramid was inspired by Zope, Pylons (version 1.0) and Django. As a result, Pyramid borrows several
concepts and features from each, combining them into a unique web framework.
Many features of Pyramid trace their origins back to Zope. Like Zope applications, Pyramid applications
can be easily extended: if you obey certain constraints, the application you produce can be reused, modified, re-integrated, or extended by third-party developers without forking the original application. The
concepts of traversal and declarative security in Pyramid were pioneered first in Zope.
The Pyramid concept of URL dispatch is inspired by the Routes system used by Pylons version 1.0. Like
Pylons version 1.0, Pyramid is mostly policy-free. It makes no assertions about which database you
should use, and its built-in templating facilities are included only for convenience. In essence, it only
supplies a mechanism to map URLs to view code, along with a set of conventions for calling those views.
You are free to use third-party components that fit your needs in your applications.
The concept of view is used by Pyramid mostly as it would be by Django. Pyramid has a documentation
culture more like Django’s than like Zope’s.
Like Pylons version 1.0, but unlike Zope, a Pyramid application developer may use completely imperative
code to perform common framework configuration tasks such as adding a view or a route. In Zope, ZCML
is typically required for similar purposes. In Grok, a Zope-based web framework, decorator objects
and class-level declarations are used for this purpose. Out of the box, Pyramid supports imperative and
decorator-based configuration; ZCML may be used via an add-on package named pyramid_zcml.
Also unlike Zope and unlike other “full-stack” frameworks such as Django, Pyramid makes no assumptions about which persistence mechanisms you should use to build an application. Zope applications are
typically reliant on ZODB; Pyramid allows you to build ZODB applications, but it has no reliance on the
ZODB software. Likewise, Django tends to assume that you want to store your application’s data in a
relational database. Pyramid makes no such assumption; it allows you to use a relational database but
doesn’t encourage or discourage the decision.
Other Python web frameworks advertise themselves as members of a class of web frameworks named
model-view-controller frameworks. Insofar as this term has been claimed to represent a class of web
frameworks, Pyramid also generally fits into this class.

```
##You Say Pyramid is MVC, But Where’s The Controller?
The Pyramid authors believe that the MVC pattern just doesn’t really fit the web very well. In a
Pyramid application, there is a resource tree, which represents the site structure, and views, which
tend to present the data stored in the resource tree and a user-defined “domain model”. However,
no facility provided by the framework actually necessarily maps to the concept of a “controller”
or “model”. So if you had to give it some acronym, I guess you’d say Pyramid is actually an
“RV” framework rather than an “MVC” framework. “MVC”, however, is close enough as a general
classification moniker for purposes of comparison with other web frameworks.
```
