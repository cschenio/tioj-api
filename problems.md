Problems
========

Methods
-------

### **GET** /problems
Return a list of problems with attributes.

####Parameters
| Field        | Format             | Description |
|--------------|--------------------|-------------|
| offset       | Integer            | The response start from the offset-th problem. |
| limit        | Integer            | The quantity of problems in this response. |
| problem_name | String             | Partial name of the problem's entire name. |
| tags         | String,String, ... | Whole name of the tags, seperated by comma. |

Attributes
----------
| Field         | Format   | Description |
|---------------|----------|-------------|
| name          | String   | The name. |
| description   | Text     | The main description of the problem. |
| source        | Text     | Denote where the problem comes from. |
| created_at    | Datetime | Time when created. |
| updated_at    | Datetime | Time last updated. |
| input         | Text     | The description of the input format. |
| output        | Text     | The description of the output format. |
| sample_input  | Text     | The sample input of the problem. |
| sample_output | Text     | The sample output of the problem. |
| hint          | Text     | The hint (if exists) to the problem solver. |
| state         | Integer  | Decided whether a problem is visible, every integer represents different state(to be completed) |
