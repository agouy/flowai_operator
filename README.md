# flowai operator

#### Description
`flowai` operator performs quality control on flowcytometry data.

##### Usage

Input projection|.
---|---
`row`   | represents the variables (e.g. channels, markers)
`col`   | represents the observations (e.g. cells, samples, individuals) 
`y-axis`| measurement value


Output relations|.
---|---
`QCvector`         | numeric, values above 10000 are considered FAIL, under 10000 PASS


##### Details

This operator is able to perform an automatic quality control on FCS data acquired using flow cytometry instruments. By evaluating three different properties: 

* flow rate
* signal acquisition
* dynamic range

The quality control enables the detection and removal of anomalies.

This operator wraps the `flowAI::flow_auto_qc` function from the [flowAI` R package](http://bioconductor.org/packages/release/bioc/html/flowAI.html)


#### Reference

[flowAI R package]((http://bioconductor.org/packages/release/bioc/html/flowAI.html))

##### See Also


#### Examples
