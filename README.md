# Student Management Dashboard

A student management dashboard built in Python to view and manage
student information, attendance, academic performance, and fee status in
one place. The project uses a CSV data file (`students_data.csv`) and
presents summary metrics, charts, a student table, and a form for adding
student records.

## Dashboard Preview

The dashboard includes these sections:

-   **Overview** --- summary cards, department-wise student chart,
    fee-status chart, and student records.
-   **Students** --- student record management.
-   **Attendance** --- attendance information.
-   **Results** --- marks and academic performance.
-   **Fees** --- fee information and payment status.

> The sections and metrics shown depend on the current implementation of
> the notebook.

## Features

-   View student records in a tabular format.
-   Search students by name or roll number.
-   Filter records by department and status.
-   View total student count.
-   View average attendance and average marks.
-   Track pending fees.
-   Visualize student counts by department using a bar chart.
-   Visualize paid versus pending fees using a pie chart.
-   Enter a student's name, roll number, department, year, attendance,
    marks, fees, and fee status through the Add Student form.
-   Use a CSV file as the student data source.

## Dashboard Summary

The screenshot shows the following example summary values:

  Metric                 Displayed value
  -------------------- -----------------
  Total Students                     240
  Average Attendance               74.7%
  Average Marks                     64.6
  Pending Fees                ₹1,830,000

These values reflect the data shown in the screenshot and may change
when the CSV data changes.

## Student Data

The dashboard uses `students_data.csv`. The visible columns include:

  Column       Description
  ------------ --------------------------------
  Roll No      Unique student roll number
  Name         Student name
  Department   Student's department
  Year         Current academic year
  Attendance   Attendance percentage or score
  Marks        Student marks
  Fees         Fee amount
  Fee Status   Paid or Pending
  Status       Active or Inactive 

The example is taken from the visible sample data in the screenshot.

## Technologies

Based on the notebook interface and visible charts, the project is
intended for a Python/Jupyter-style environment. The likely libraries
and file format are:

-   **Python** --- application logic.
-   **Pandas** --- reading and working with tabular student data, if
    used in the notebook.
-   **Matplotlib** --- charts and visualizations, if used in the
    notebook.
-   **CSV** --- student data storage.
-   **Jupyter Notebook** --- interactive notebook interface.

Confirm the notebook imports before finalizing the dependency list.

## Project Files

A suggested project layout is:

``` text
Student-Management-System/
├── Student management system.ipynb
├── students_data.csv
└── README.md
```

Use the actual notebook filename if it differs from the example above.

## Setup and Run

1.  Keep the notebook and `students_data.csv` in the same folder, unless
    the notebook uses a different file path.
2.  Open the notebook in a Jupyter-compatible environment.
3.  Make sure the libraries imported by the notebook are available.
4.  Run the notebook cells in order.
5.  Check that `students_data.csv` loads successfully and that the
    dashboard renders.

If the project uses Pandas and Matplotlib, they can normally be
installed in a standard Python environment with:

``` bash
python -m pip install pandas matplotlib
```

If the notebook uses interactive widgets, install any additional
packages required by its imports. Package installation can differ in
browser-based or Pyodide environments.

## Using the Dashboard

1.  Open the **Overview** section to review the summary cards and
    charts.
2.  Enter a student's name or roll number in the search field to find a
    record.
3.  Select a department or status from the dropdown filters.
4.  Review department counts and the fee-status chart.
5.  Use the student form to enter the required details and select **Add
    Student**, if that action is implemented in the notebook.
6.  Open the Students, Attendance, Results, or Fees section to review
    the corresponding information.

## Data and Validation Notes

-   Each student should have a unique roll number.
-   Attendance and marks should use the ranges expected by the notebook,
    commonly 0--100.
-   Fee amounts should be numeric.
-   Fee Status should use consistent values such as `Paid` and
    `Pending`.
-   Status should use consistent values such as `Active` and `Inactive`.
-   Keep a backup of `students_data.csv` before making bulk changes.

## Future Improvements

Possible extensions include:

-   Edit and delete student records.
-   Input validation and duplicate roll-number checks.
-   Export filtered records to CSV or Excel.
-   Student-wise result and attendance reports.
-   Charts that update automatically after data changes.
-   Persistent saving when a new student is added.
-   Login and role-based access for administrators and staff.
-   Responsive web deployment.

## Author

**Project:** Student Management Dashboard\
**Data file:** `students_data.csv`

## License

No license is specified for this project yet. Add a `LICENSE` file if
you plan to publish or distribute it.
