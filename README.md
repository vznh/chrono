# Chronolex
Chronolex is meant for fast and meticulous mass calendar planning. 

## ( ͡° ͜ʖ ͡°)つ📱
You can utilize **Chronolex** easily using natural language planning. You can also be as detailed or as broad as you'd like. **Chronolex** will never heavily assume anything. If you prefer, **Chronolex** will ask follow-up questions in order to make more educated calendar entries.    

For example, 

__Most ideal input__
```xml
<INPUT>
chaos theory mwf 8a to 9a at natural sciences 1 room 111 for 10 weeks
</INPUT>

<EXPECTED_OUTPUT>
<Event>
{
  name: "Chaos Theory",
  days: ["MON", "WED", "FRI"],
  location: "Natural Sciences 1",
  room: "111"
  recurring: {
    "freq": "weekly",
    "byday": ["MO", "WE", "FR"],
    "count": 30
  }
}
</Event>
</EXPECTED_OUTPUT>
```

__Least ideal and contextual input__
```xml
<INPUT>
chaos theory
</INPUT>

<EXPECTED_OUTPUT>
[Option to place as a to-do item instead of a calendar event]
[Optional] What time does it start and end? Where will it be located? Is this a recurring event? 
</EXPECTED_OUTPUT>
```

__Assumption of events__
```xml
<INPUT>
chaos theory natural sciences 1 
</INPUT>

<EXPECTED_OUTPUT>
<To-do>
{
  name: "Chaos Theory",
  location: "Natural Sciences 1"
}
</To-do>
</EXPECTED_OUTPUT>
```

## ( ͡° ʖ ͡°)つ💻
Chronolex **never** remembers any events from your calendar. 
We store the following — 
* Your email and name (which you can delete from our server at any time, no fuss)
* Your preferences
* Previous raw entries
* Queued events that you've injected (for 30 days)
* Your token usage
* Deleted to-dos (which you can delete from our server forever, willingly)

## ( つ ◕_◕ )つ━☆💸
Chronolex's basic capabilities (such as mass planning) will always be free. There might be features where Chronolex will have to go paid, but it will never obstruct the usage of free and fast planning.

