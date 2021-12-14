<template>
  <div id="app">
    <full-calendar :events="events"></full-calendar>
  </div>
</template>

<script>
//https://github.com/CroudTech/vue-fullcalendar
import { FullCalendar } from 'vue-full-calendar'
import 'fullcalendar/dist/fullcalendar.css'

export default {
  components: {
    FullCalendar,
  },
  data() {
    return {
      events: [
        {
            title  : 'event1',
            start  : '2021-12-01',
            color: 'yellow',
          textColor: 'black',
        },
        {
            title  : 'event2',
            start  : '2021-12-05',
            end    : '2021-12-07',
                      color: 'red',
        },
        {
            title  : 'event3',
            start  : '2021-12-09T12:30:00',
            allDay : false,
        },
      ]
    }
  }
}
</script>

