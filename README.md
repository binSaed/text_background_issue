# text_background_issue

## Steps to repreduce
Flutter 3.35.2 • channel stable  

```dart
Text(
          'Test',
          style:
          TextStyle(
            fontSize: 24,
            background: Paint()
              ..strokeWidth = 44
              ..color = const Color(0x1a0078ff)
              ..style = PaintingStyle.stroke
              ..strokeJoin = StrokeJoin.round,
          ),
        )
```

```
flutter run
```

<img width="1920" height="1080" alt="Screenshot 2025-08-27 at 8 34 41 PM" src="https://github.com/user-attachments/assets/60dafda5-d595-4444-a0ef-75af3da05d80" />
