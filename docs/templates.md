# Templates

The Flask-vuejs extension create for you a `base.html` template. However, is necessary
inherit from this template. This section shows you how to do this.

## Creating your base template

In your `base.html` template use the extends block for inherit from `vue/base.html`

```jinja
{% extends 'vue/base.html' %}
```

This is enough for the work application. But, You may want to use the components inside the `.html` or `.jinja` files, 
this will be necessary when you don't want to create a separate `vue` application from the `backend`.

To do this, use the content block to start the block and then place the component inside,

```html
{% extends 'vue/base.html' %}

{% block content %}
    <hello-world :name="Pacotei"></hello-world>
{% endblock %}
```

When you do this, you will receive a message on the web like this: `Hello Pacotei`. 

Verify in [http://localhost:5000](http://localhost:5000). 

## Demo

You can see a [demo](https://github.com/pacotei/flask-vuejs/blob/master/sample_app/templates/form.html)