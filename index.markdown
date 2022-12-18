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
<A HREF="https://www.vdst.de/wp-content/uploads/VDST-DTSA-Ordnung-2021.pdf#page=28">Voraussetzungen für Gold</a>

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
	  JA ({{ person.AKNTG }})
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
  </tr>
  {% endif %}
{% endfor %}
</table>

<h1> Silber </h1> 
<A HREF="https://www.vdst.de/wp-content/uploads/VDST-DTSA-Ordnung-2021.pdf#page=25">Voraussetzungen für Silber</a>
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

<h1> Bronze </h1> 
<A HREF="https://www.vdst.de/wp-content/uploads/VDST-DTSA-Ordnung-2021.pdf#page=22">Voraussetzungen für Bronze</a>
<table id="tg-FK3W8" class="tg">
  <tr>
    <th>Name</th>
    <th>Nächstes Brevet</th>
    <th>Tauchtauglichkeit</th>
    <th>AK HLW</th>
  </tr>

{% for person in site.data.kandidaten%}
  {% if person.brevet=="Bronze" %}
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
    <td> 
	{% if person.AKHLW %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
  </tr>
  {% endif %}
{% endfor %}
</table>

<h1> KTA Gold </h1> 
<A HREF="https://www.vdst.de/wp-content/uploads/VDST-KTSA-Ordnung-2021.pdf#page=18">Voraussetzungen für KTA Gold</a>
<table id="tg-FK3W8" class="tg">
  <tr>
    <th>Name</th>
    <th>Nächstes Brevet</th>
    <th>Tauchtauglichkeit</th>
    <th>KSK GF </th>
  </tr>

{% for person in site.data.kandidaten%}
  {% if person.brevet=="KTA Gold" %}
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
    <td> 
	{% if person.GF %} 
	  JA 
      	{% else %} 
	  NEIN
      	{% endif %} 
    </td> 
  </tr>
  {% endif %}
{% endfor %}
</table>

<h1> Schnorchelabzeiichen Otter </h1>


<A HREF="https://www.vdst.de/wp-content/uploads/VDST-KTSA-Ordnung-2021.pdf#page=8">Voraussetzungen für SA Otter</a>
<table id="tg-FK3W8" class="tg">
  <tr>
    <th>Name</th>
    <th>Nächstes Brevet</th>
    <th>Ärztl Bescheinigung</th>
  </tr>

{% for person in site.data.kandidaten%}
  {% if person.brevet=="Otter" %}
    <tr> 
    <td> {{person.name}}</td>, 
    <td> {{person.brevet}}</td> 
    <td>
      {% if person.ttg %} 
	  JA 
      {% else %} 
	  NEIN
      {% endif %} 
    </td>
  </tr>
  {% endif %}
{% endfor %}
</table>
