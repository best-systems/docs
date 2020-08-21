![](img/update-banner.png)
# Release Update

## 20170731 Core - Update - Job service POM build, Javascript bug
- **Job service use POM** to build and use the same model of App model
- **Javascript running after DOM** loading to avoid script loading problem. The javascript sometime did not load correctly because it run before DOM loaading, so the scrip can not find Id componenwt. The new fix solve this problem. Now the javascrip always load after DOM finishes. Solution from [Vaadin, JS and DOM initialization order](https://vaadin.com/blog/-/blogs/vaadin-js-and-dom-initialization-order)
- Add SSL to images.best.systems
- Add new role menu/custom to make custome menu. Some user like sales need compact menu . This option help the the menu of sales compact
- Scroll to focus field (mobile view)
- New role: Import, Export for all entities
- Sending emails when creating user (mporting employees)
- Add Sync MYOB button and job
- Fix bugs: Auto complete component, Dropdown component
- Default sort allows many columns
- Code: Add parameters to Show/hide message when job running.

Project applied:

- Thang Long CRM

TODO:

- Review java memory and performance (Profiler with VisualVM, jmap, jhat)


## 20170627 Core - Update - Show real IP fo client when the app behind the proxy
- Log file Bestsystem shows correct IP and user login
- Audit log show correct user and IP login

**TODO:**

- Retrict login by IP

## 20170620 Form module - Update - Printing form to PDF file

- Printing all forms to PDF
- Using FOP library to print form

**Installation note**

- The font folder is copied at `/appdata/fonts`
- Need to run with Oracle Java for export PDF with fonts.

**Applied** Cesti ce-statistics

**TODO:**

- Apply to Bach Khoa