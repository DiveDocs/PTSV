---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<h1>Planung Tauchausbildung 2023</h1>

<head>
<style>
table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 80%;
}

td, th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #dddddd;
}
</style>
</head>


<h1> Voraussetzungen </h1> 
<h2> Gold </h2> 
<table id="tg-FK3W8" class="tg">
  <tr>
    <th>Name</th>
    <th>Nächstes Brevet</th>
    <th>Tauchtauglichkeit</th>
    <th>Anzahl TG </th>
    <th>(davon 30m-40m)</th>
    <th>AK TSR</th>
    <th>AK NTG / ProblemLösen</th>

  </tr>
{% for person in site.data.kandidaten%}
  {% if person.brevet=="Gold" %}
    <tr> 
    <td> {{person.name}}</td>, 
    <td> {{person.brevet}}</td> 
    <td>
      {% if person.ttg %} 
	  JA (gültig bis: {{person.gueltig}} )
      {% else %} 
	  NEIN
      {% endif %} 
    </td>
    <td> {{person.TG}}</td> 
    <td> {{person.TGTief}}</td> 
    <td> 
	{% if person.AKTSR %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
    <td> 
	{% if person.AKNTG %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
  </tr>
  {% endif %}
{% endfor %}
</table>

<h1> Silber </h1> 
<table id="tg-FK3W8" class="tg">
  <tr>
    <th>Name</th>
    <th>Nächstes Brevet</th>
    <th>Tauchtauglichkeit</th>
    <th>Anzahl TG </th>
    <th>(davon 15m-25m )</th>
    <th>AK OT</th>
    <th>AK GF </th>
    <th>AK MB</th>
    <th>AK HLW</th>

  </tr>
{% for person in site.data.kandidaten%}
  {% if person.brevet=="Silber" %}
    <tr> 
    <td> {{person.name}}</td>, 
    <td> {{person.brevet}}</td> 
    <td>
      {% if person.ttg %} 
	  JA (gültig bis: {{person.gueltig}} )
      {% else %} 
	  NEIN
      {% endif %} 
    </td>
    <td> {{person.TG}}</td> 
    <td> {{person.TGTief}}</td> 
    <td> 
	{% if person.AKOT %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
    <td> 
	{% if person.AKGF %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
    <td> 
	{% if person.AKHLW %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
    <td> 
	{% if person.AKMB %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
  </tr>
  {% endif %}
{% endfor %}
</table>
