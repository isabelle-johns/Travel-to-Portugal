![header-portugal](https://user-images.githubusercontent.com/73572478/97767372-c546bf80-1b6f-11eb-8aa5-55632cab228f.jpg)

<div class="tabcontrol container">
    <ul class="tabcontrol tabs" style="{{include.headerstyle}}">
        {% for tab in include.tabs %}
            <li class="tabcontrol tab {% if {tab[1].active %}active{% endif %}" data-name="{{tab[1].name}}" data-target="tab_{{include.id}}" data-source="{{include.id}}__{{tab[1].source}}">
                {{tab[1].title}}
            </li>
            {% if tab[1].active %}
                {% assign defaultsource = tab[1].source %}
            {% endif %}
            {% if tab[1].content %}
            <div id="{{include.id}}__{{tab[1].source}}" class="hidden">
                {{tab[1].content | markdownify }}
            </div>
            {% endif %}
        {% endfor %}
    </ul>
    <div id="tab_{{include.id}}" class="tabcontrol body {{include.bodyclass}}" style="{{include.bodystyle}}" data-defaultsource="{{include.id}}__{{defaultsource}}">
    </div>
</div>

tabs: 
    tab1:
        name: foo
        title: Page One
        source: source1
    tab2:
        name: bar
        title: Page Two
        source: source2
        content: >
            ## Headline

            A Link: [link](https://foo.bar.org)
    tab3:
        name: baz
        title: Page Three
        active: 1
        source: source3

## _What does Portugal have to offer?_

Portugal, located in South Europe and bordering Spain is a unique country with a variety of activities, historical buildings, intangible heritage and spectacular views. Whether it's the indulgent cuisine, pristine beaches or history that date back thousands of years, Portugal will not fail to entertain you.

## _A perfect spot for young people_
Portugal is the whole package for young adults who like to travel. For the risktakers and adrenaline seekers, the _Pena Adventura Park_ is the way to go with it's extreme ziplining activity over a vast, beautiful landscape. There is also a variety of different escape rooms and waterparks. But if you're looking for something a little more historical, Portugal has immense diversification of galleries, museums and fortresses you can visit. Contrastingly, if you're just looking for a place to repose or kick-back, beaches such as _Praia da Marinha_ or _Praia de São Rafael_ will have you soaking up the sun for hours. 

![image](https://user-images.githubusercontent.com/73572478/97794470-af5bfc00-1c4e-11eb-9ff9-334a5be291b6.png)

## _Precautions and warnings before travelling_
Like every other holiday destination, precautions have to be taken into account when visiting somewhere new. Better to be safe than sorry.

### Safety

- Bushfires occur in the summertime
- Drink spiking is common; so do not leave your drink unattended
- Bag snatching, pickpocketing occur on beaches, public transport and tourist hot-spots. Do not leave your belongings unattended.

### Local Laws
- Always carry photo identification or ID                                                                                           
- Gambling is only legal in licensed venues
- Posession or use of illegal drugs will attract large fines

### Health
- Medical treatment is expensive (no reciprocal healthcare agreement between Portugal and Australia)
- May need an import permit to get medication by post

### Local Contacts
When in trouble, the _Consular Services Charter_ details what the Australian Government can assist you with overseas. If you are seeking consular assistance, you should visit or contact the Australian Embassy in Lisbon. 
- [visit the Portugal Australian Embassy website Here](http://www.portugal.embassy.gov.au/lbon/home.html)
- email; ausemb.lisbon@dfat.gov.au

![download](https://user-images.githubusercontent.com/73572478/97767242-08546300-1b6f-11eb-8033-72fca4e229b2.jpg) ![download](https://user-images.githubusercontent.com/73572478/97767418-03dc7a00-1b70-11eb-98b7-c4309794e4bc.jpg)


### _Support or Contact_

Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
