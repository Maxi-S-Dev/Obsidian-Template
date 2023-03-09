---
tags: goal
alias: Develop 5 Apps
Type: Professional
Progress: 0
Target: 2
Reason: Learn to develop Apps and stay motivated
Timespan:
     1 Year
---

%%
Bar:: `$= dv.view('progress-bar', {file: '2023-03-04 - Develop 5 Apps'})`
Projects:: `$= const projects = dv.page('2023-03-04 - Develop 5 Apps').file.inlinks.where(p => { const mp = dv.page(p.path); return mp.tags?.includes('project') && mp.status === 'In Progress'}); if (projects.length > 0) { dv.header(4, projects.length > 1 ? "Projects" : "Project"); dv.list(projects) }`
%%

## What does success look like? What are the key results?

-

## Related core values

-

## Projects to make this happen

### Ideas

-

### Created projects

```dataviewjs
const pages = dv.current().file.inlinks.where(p => dv.page(p.path).tags?.includes('project'));

dv.table(["Project", "Status"], pages.map(p => {
	const page = dv.page(p.path);
	return [page.file.link, page.status]
}));
```
