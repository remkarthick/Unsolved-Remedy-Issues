# 1. DWP Catalog request returns Fault status with error "item with name 0 is not found
- While submitting a DWP Catalog request, it got created with a fault status. The error displayed was item with name 0 is not found.
- [x] Answer : Issue is due to the qualification. Check the qualification under the exclusive gateway.

# 2. Issue with Sub-Process within a Sub-Process
- I have created an workflow containing a Sub-Process(Sequential Multi Instance) that loops on a multi select table field. Within the fore mentioned Sub-Process i have created another Sub-Process(Sequential Multi Instance) that loops on another multi select table field.
- Now the problem is, the child sub process behaves independent of the parent sub process. i.e. it its not tied to the variables passed as part of the parents looping instance. Is it a normal behavior or is it a bug?
- [x] Answer : The Child Sub Process acts like a parallel process rather than a sequential process which is reason for this issue.
