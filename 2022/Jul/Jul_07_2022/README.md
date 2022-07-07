# Notes for Jul_07_2022

This is a note or a diary for the things I research in a day, this note intended for me not to forget the knowlegde I has gain (or things I has read).

## D3 Security SOAR Command Notes 

Link: <https://jinja.palletsprojects.com/en/2.11.x/templates/#list-of-control-structures>

So if you are using SOAR from D3 Security SOAR then you in luck because this is the only guide that you will see if you trying to search for tutorial and guide
The first thing you will go to the Task Data Formatter and read it right away because it help you a tons

The language or the template it used is **Jinja** which is a template designer use in Python, the link above is the specification of it, basically it is like Python

- You want to **set variable and assign** use {% %} 
- You want to do **some calculation**  or **print** use {{ }} -> quite anoying to use this command or print format you should use format() (not useful tbh)
and I if you want to get rid of whitespace and newline you should use {%- -%} or (see the diffence) adding "-" or "+" to a block of code with do the trick

Example: 

```Jinja
  {%- for event in events -%}
    {% set event_time_diff = (event.intakeTime | datetime_diff(current_times, 'seconds')) | divide_by(3600)) %}
    {%- if event_time_diff >= 4.0 -%}
      {{- event.ID -}}
    {%- event.ID -%}
  {% endfor %}

```

I do this because the trailing white space and newline

**Create List and Append to it**

```Jinja
  {% set sample_list = []  %}
  {{ sample_list.append(sample_data)}}

```

