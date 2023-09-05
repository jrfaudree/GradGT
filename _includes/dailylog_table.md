{% assign data = include.data %}
<table class="asst-table">
{% for dailylog in data.dailylog %}
<tr>
  <td><a href="{{ data.home }}/{{ dailylog.url }}"><b>{{ dailylog.name }}</b></a> &nbsp; &nbsp; Date {{ dailylog.date }}&nbsp; &nbsp; <a href="{{ data.home }}/{{ dailylog.url }}"><b>{{ video }}</b></a>.
  </td>
</tr>
{% endfor %}
</table>
