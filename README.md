# Core Development App
Task management application for developers on MVC. This application was developed by me for a YouTube channel subscriber in 2020.

Аn ASP.NET MVC application. It displays a table of data representing "requests", with columns for ID, name, category, deadline, description, email, and edit/delete buttons. The table data is populated using a ViewBag variable named "OnePageOfProducts", which is cast to an IPagedList using the HTML Helper from the X.PagedList.Mvc.Core namespace.

In addition to the table, the view includes a title, a responsive wrapper div, and a paging control generated by the PagedListPager HTML Helper. There is also a conditional statement that sets the value of a variable named "selecList" based on whether TempData contains a key called "selectListdata". If it does, the value of "selectListdata" is cast as an IEnumerable of ApplicationListModel and assigned to "selecList"; otherwise, "selecList" is set to null.

Overall, the view appears to be designed to allow users to view, edit, and delete requests, with support for paging and category selection using the "selecList" variable.
