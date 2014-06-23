###  Pyramid Web 框架

Pyramid is a small, fast, down-to-earth Python web framework. It is developed as part of the Pylons Project. It is licensed under a BSD-like license.

```python
1 from pyramid.view import view_config
2
3 @view_config(renderer=’templates/mytemplate.txt’)
4 def my_view(request):
5 return {’name’:’world’}
>>>>>>> 221a89ab191f2b3e4fd361f901194cec7d0d6d39
```
When the template is rendered, it will show:
Hello, world!
See also Built-In Renderers for more general information about renderers, including Chameleon text
renderers.
![](https://developer.apple.com/library/prerelease/ios/documentation/Swift/Conceptual/Swift_Programming_Language/Art/stackPoppedOneString_2x.png)
