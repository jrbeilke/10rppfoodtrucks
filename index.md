---
layout: default
---

<link href='https://unpkg.com/@fullcalendar/core@4.2.0/main.css' rel='stylesheet' />
<link href='https://unpkg.com/@fullcalendar/list@4.2.0/main.css' rel='stylesheet' />

<script src='https://unpkg.com/@fullcalendar/core@4.2.0/main.js'></script>
<script src='https://unpkg.com/@fullcalendar/list@4.2.0/main.js'></script>
<script src='https://unpkg.com/@fullcalendar/google-calendar@4.2.0/main.js'></script>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    var calendarEl = document.getElementById('calendar');

    var calendar = new FullCalendar.Calendar(calendarEl, {
      plugins: [ 'googleCalendar', 'list' ],
      defaultView: 'listDay',
      events: {
        googleCalendarId: 'gh6rricliekd9qm2j1ik3q963c@group.calendar.google.com'
      },
      googleCalendarApiKey: 'AIzaSyC2-WyAt_e0eQMfqEpegOvfqi2661_l-jk',
      header: {
        left:   'prev,next',
        center: '',
        right:  'today'
      },
      height: 'auto',
      listDayFormat: {
        year: 'numeric',
        month: 'long',
        day: 'numeric',
        weekday: 'long'
      }
    });

    calendar.render();
  });
</script>

# What's for Lunch?

Here are the food trucks we know about that are planning to be at 10RPP:

[10RPP Food Trucks Calendar](https://calendar.google.com/calendar/embed?src=gh6rricliekd9qm2j1ik3q963c%40group.calendar.google.com&ctz=America%2FChicago&mode=AGENDA)

<div id='calendar'></div>
