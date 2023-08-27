{% assign data = include.data %}
<table class="asst-table">
{% for homework in data.homework %}
<tr>
  <td><b>{{ homework.name }}</b> &nbsp; &nbsp; Due {{ homework.due }}.<br><br>
    
    {% if homework.url %}
      <table class="inner">
        <tr>
          <td><a href="{{ data.home }}/{{ homework.override }}"></td>
        <\tr>
      </table>
    {% endif %}
  </td>
</tr>
{% endfor %}
</table>
