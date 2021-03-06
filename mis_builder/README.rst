.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
    :alt: License: AGPL-3

===========
MIS Builder
===========

This module allows you to build Management Information Systems dashboards.
Such style of reports presents KPI in rows and time periods in columns.
Reports mainly fetch data from account moves, but can also combine data coming
from arbitrary Odoo models. Reports can be exported to PDF, Excel and they
can be added to Odoo dashboards.

Installation
============

There is no specific installation procedure for this module.

Configuration and Usage
=======================

To configure this module, you need to:

* Go to Accounting > Configuration > Financial Reports > MIS Report Templates where
  you can create report templates by defining KPI's. KPI's constitute the rows of your
  reports. Such report templates are time independent.

.. figure:: static/description/ex_report_template.png
   :scale: 80 %
   :alt: Sample report template

* Then in Accounting > Reporting > MIS Reports you can create report instance by
  binding the templates to time period, hence defining the columns of your reports.

.. figure:: static/description/ex_report.png
   :alt: Sample report configuration

* From the MIS Report view, you can preview the report, add it to and Odoo dashboard,
  and export it to PDF or Excel.

.. figure:: static/description/ex_dashboard.png
   :alt: Sample dashboard view

For further information, please visit:

* https://www.odoo.com/forum/help-1

Known issues / Roadmap
======================

* More tests should be added. The first part is creating test data, then it will be
  easier. At the minimum, We need the following test data:

  * one account charts with a few normal accounts and view accounts,
  * two fiscal years,
  * an opening entry in the second fiscal year,
  * to test multi-company consolidation, we need a second company with it's own
    account chart and two fiscal years, but without opening entry; we also need
    a third company which is the parent of the other two and has a consolidation
    chart of account.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/account-financial-reporting/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed feedback
`here <https://github.com/OCA/account-financial-reporting/issues/new?body=module:%20mis_builder%0Aversion:%208.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Credits
=======

Contributors
------------

* Stéphane Bidoul <stephane.bidoul@acsone.eu>
* Laetitia Gangloff <laetitia.gangloff@acsone.eu>
* Adrien Peiffer <adrien.peiffer@acsone.eu>

Maintainer
----------

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit http://odoo-community.org.
