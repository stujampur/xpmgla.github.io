---
layout: contributors
title: Contributors
---

<div class="contributors">
{% for author in site.data.authors %}
    {% if author[1].showInList != false %}
    <div class="contributor"><hr/>
        {% if author[1].avatar %}<img src="{{ site.baseurl }}/images/members/{{ author[1].avatar }}" alt="author[1].image" />{% endif %}

        <!--<img src="{{ site.baseurl }}/images/members/{{ author[1].avatar }}" alt="author[1].image" />-->
        <div class="meta">

            <p> <h2>{{ author[1].name | default: "No Name Specified"}} {% if author[1].alias %}<small>[{{ author[1].alias }}]</small>{% endif %}</h2>
                {% if author[1].role %}<strong>{{ author[1].role }}</strong><br/>{% endif %}
                {% if author[1].role %}<a href="{{ author[1].website }}" target="_blank">{{ author[1].website }}</a><br/>{% endif %}
                {% if author[1].role %}<a href="mailto:{{ author[1].email }}">{{ author[1].email }}</a>{% endif %}
            </p>
            <p>
            {% if author[1].bio %}<strong>Bio:&nbsp;</strong>{{ author[1].bio }}<br/>{% endif %}
            </p>
            <p>
            {% if author[1].interests %}<strong>Interests:</strong>{{ author[1].interests }}<br/>{% endif %}
            </p>
            <p>Social:
                {% assign hasSocialMediaIcon=false %}
                {% if author[1].twitter %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://twitter.com/{{ author[1].twitter }}"><i class="fa fa-twitter"></i></a>&nbsp;@<a target="_blank" href="http://twitter.com/{{ author[1].twitter }}">{{ author[1].twitter }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].github %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://github.com/{{ author[1].github }}"><i class="fa fa-github"></i></a>&nbsp;<a target="_blank" href="http://github.com/{{ author[1].github }}">{{ author[1].github }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].facebook %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://facebook.com/{{ author[1].facebook }}"><i class="fa fa-facebook"></i></a>&nbsp;<a target="_blank" href="http://facebook.com/{{ author[1].facebook }}">{{ author[1].facebook }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].youtube %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://youtube.com/{{ author[1].youtube }}"><i class="fa fa-youtube"></i></a>&nbsp;<a target="_blank" href="http://youtube.com/{{ author[1].youtube }}">{{ author[1].youtube }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].deviant %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://deviantart.com/{{ author[1].deviant }}"><i class="fa fa-deviantart"></i></a>&nbsp;<a target="_blank" href="http://deviantart.com/{{ author[1].deviant }}">{{ author[1].deviant }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].instagram %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://instagram.com/{{ author[1].instagram }}"><i class="fa fa-instagram"></i></a>&nbsp;<a target="_blank" href="http://instagram.com/{{ author[1].instagram }}">{{ author[1].instagram }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].googleplus %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://googleplus.com/{{ author[1].googleplus }}"><i class="fa fa-google-plus"></i></a>&nbsp;<a target="_blank" href="http://googleplus.com/{{ author[1].googleplus }}">{{ author[1].googleplus }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].linkedin %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://linkedin.com/in/{{ author[1].linkedin }}"><i class="fa fa-linkedin"></i></a>&nbsp;<a target="_blank" href="http://linkedin.com/in/{{ author[1].linkedin }}">{{ author[1].linkedin }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% if author[1].pinterest %}{% if hasSocialMediaIcon %} | {% endif %}<a target="_blank" href="http://pinterest.com/{{ author[1].pinterest }}"><i class="fa fa-pinterest"></i></a>&nbsp;<a target="_blank" href="http://pinterest.com/{{ author[1].pinterest }}">{{ author[1].pinterest }}</a>{% assign hasSocialMediaIcon=true %}{% endif %}
                {% unless hasSocialMediaIcon %}No links specified.{% endunless %}
            </p>
        </div>
    </div>
    {% endif %}
{% endfor %}
<br/><br/>

</div>
