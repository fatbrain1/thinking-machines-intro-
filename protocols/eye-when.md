# EYE–WHEN Protocol
## Gaze-Driven Engagement

Implementation:
```python
class EyeWhen:
    def __init__(self):
        self.attention_score = 0
        
    def update(self, gaze_data):
        self.attention_score = 0.7*gaze_data.focus + 0.3*gaze_data.blink_rate
