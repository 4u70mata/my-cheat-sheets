### Django Template Language Cheat Sheet  

1. Variable Output:
   ```django
   {{ variable_name }}
   ```

2. Template Tags:
   ```django
   {% tag_name %}
   ```

3. Comments:
   ```django
   {# This is a comment #}
   ```

4. Filters:
   ```django
   {{ variable|filter_name }}
   ```

5. Common Filters:
   ```django
   {{ name|upper }}
   {{ text|truncatewords:30 }}
   {{ date|date:"Y-m-d" }}
   {{ value|default:"N/A" }}
   ```

6. Control Structures:
   ```django
   {% if condition %}...{% endif %}
   {% for item in list %}...{% endfor %}
   ```

7. Template Inheritance:
   Base template:
   ```django
   {% block blockname %}{% endblock %}
   ```
   Child template:
   ```django
   {% extends "base.html" %}
   ```

8. Including Templates:
   ```django
   {% include "snippet.html" %}
   ```

9. URL Routing:
   ```django
   {% url 'name_of_view' %}
   ```

10. CSRF Token:
    ```django
    {% csrf_token %}
    ```

11. Static Files:
    ```django
    {% load static %}
    <img src="{% static 'image.jpg' %}">
    ```

12. Custom Template Tags:
    ```django
    {% load custom_tags %}
    {% custom_tag %}
    ```
