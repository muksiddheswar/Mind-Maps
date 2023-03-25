# Object composition

### Aggregation vs Composition
- Aggregation differs from ordinary composition in that it does not imply ownership. 
- In composition, when the owning object is destroyed, so are the contained objects. 
- In aggregation, this is not necessarily true. 

For example:

```
A university owns various departments (e.g., chemistry), and each department has a number of professors. 
If the university closes, the departments will no longer exist, but the professors in those departments will continue to exist. 
Therefore, a university can be seen as a composition of departments, whereas departments have an aggregation of professors. 
In addition, a professor could work in more than one department, but a department could not be part of more than one university.

```