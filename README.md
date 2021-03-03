# yg-gantt-chart
yaml-graph Gantt Chart

Code based on https://developers.google.com/chart/interactive/docs/gallery/ganttchart

```bash
docker run -it -p7474:7474 -p7687:7687 -v $(PWD)/definition:/home/ymlgraph/definition -v $(PWD)/report:/home/ymlgraph/report nextmetaphor/yaml-graph

yaml-graph load
yaml-graph report --load -f report/fields.yaml -t report/template.gohtml > report/output.html 
```