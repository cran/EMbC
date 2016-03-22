# EMbC 1.9.4

## Bug fixes

  - When working with *move* objects, version 1.9.3 was picking GMT timestamps instead of using study local timestamps. This has been changed in version 1.9.4. because, otherwise, the solar position covarite (if used) was not conveying the right information. Of note: there is an example in the vignette illustrating the use of *move* objects that is affected by this error. Besides of illustrating the use of a *move* object, this example also depicts a case that exceptionally occurs when there is a discrepancy between the binary and the maximum likelihood partitions of the data, that results in the algorithm getting stuck in a cycle. Interestingly, this problem dissapears when the correct (local) timestaps are used. However, I decided not to rewrite the example in order not to miss the opportunity to explain this exceptional eventuallity.
  
## Minor improvements

  - The command *view* was depicting the trajectory without taking into account the proportionality of the axes. This has been corrected in version 1.9.4.
  
  - Commands *view()* and *sctr()* (in the multivariate case) depict plots that by default are using a light-grey background colour to enhance the visibility of the data points. We added a *bg* parameter that allows the user to change this default behaviour.
