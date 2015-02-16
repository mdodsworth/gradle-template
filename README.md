I've had to do this so many times, may as well have a template.

```bash
wget https://github.com/mdodsworth/gradle-template/archive/v1.0.tar.gz
tar xfz v1.0.tar.gz
rm v1.0.tar.gz
mv gradle-template-1.0/ <project name>
cd <project name>
find . -name '*.gradle' -print0 | xargs -0 sed -i '' -e 's/project-name/<project name>/g'
```
