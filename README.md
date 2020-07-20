# Table Calendar

[![Pub Package](https://img.shields.io/pub/v/table_calendar.svg?style=flat-square)](https://pub.dartlang.org/packages/table_calendar)
[![Awesome Flutter](https://img.shields.io/badge/Awesome-Flutter-52bdeb.svg?longCache=true&style=flat-square)](https://github.com/Solido/awesome-flutter)

Header will build below the Date Grid.
Custom Control On Right and Left Button Tapped in Header.


### Installation

Add to pubspec.yaml:

```yaml
dependencies:
  table_calendar:
    git:
      url: https://github.com/thelazyone11/table_calendar
```

Then import it to your project:

```dart
import 'package:table_calendar/table_calendar.dart';
```

And finally create the **TableCalendar** with a `CalendarController`:

```dart
@override
void initState() {
  super.initState();
  _calendarController = CalendarController();
}

@override
void dispose() {
  _calendarController.dispose();
  super.dispose();
}

@override
Widget build(BuildContext context) {
  return TableCalendar(
    calendarController: _calendarController,
  );
}
```

