### django-activity-stream
---
https://github.com/justquick/django-activity-stream

```py
// actstream/migrations/0003_add_follow_flag.py
from __future__ import unicode_literals
from django.db import migrations, models

class Migration(migrations.Migration):
  
  dependencies = [
    ('actream', '0002_remove_action_data'),
  ]
  
  operations = [
    migrations.AddField(
      model_name='follow',
      name='flag',
      field=models.CharField(blank=True, db_index=True, default='', max_length=255),
    ),
    migrations.AlterUniqueTogether(
      name='follow',
      unique_together=set([('user', 'content_type', 'object_id', 'flag')]),
    ),
  ]
```

```
```

```
```

