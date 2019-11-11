# SPL-FESG-Examples

In this repository, examples of product lines have been modelled by using Featured Event Sequence Graphs (FESG). A Featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). The core of the product line represents the common behavior which exists in all products that belong to the product line. The core behavior is modelled using core ESG (c-ESG). An optional behavior is modelled using a feature ESG (f-ESG).

A Featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences. In the most basic, this approach generates the event sequences of the core ESG and the feature ESGs and then, it composes these event sequences to generate a product configuration's event sequences. The sequences are composed thanks to the connection points i.e., (esgName,eventName) in the feature ESG(f-ESG) models' events.

To examine the examples and download the ESG files you can click the links below. The downloaded ESG models could be run on [Test Suite Designer](http://download.ivknet.de/) tool.

[Bank Account Product Line](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccountProductLine.md) [1] \
[Email Product Line](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/EmailProductLine.md) [2] \
[Elevator Product Line](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/ElevatorProductLine.md) [3]


## References

[1] Bank Account Product Line: http://spl2go.cs.ovgu.de/projects/23 (retrieved on 2019, November 11) \
[1] T. Thüm, I. Schaefer, S. Apel and M.Hentschel, "Family-Based Deductive Verification of Software Product Lines", 2012 Proceedings of the 11th International Conference on Generative Programming and Component Engineering, GPCE'12. 48. doi: 10.1145/2371401.2371404. \
[2] Email Product Line: http://spl2go.cs.ovgu.de/projects/17 (retrieved on 2019, November 11) \
[3] Elevator Product Line: http://spl2go.cs.ovgu.de/projects/16 (retrieved on 2019, November 11) \
[2,3] S. Apel, H. Speidel, P. Wendler, A. von Rhein and D. Beyer, "Detection of feature interactions using feature-aware verification," 2011 26th IEEE/ACM International Conference on Automated Software Engineering (ASE 2011), Lawrence, KS, 2011, pp. 372-375. doi: 10.1109/ASE.2011.6100075 \
[2,3] S. Apel, A. von Rhein, P. Wendler, A. Größlinger and D. Beyer, "Strategies for product-line verification: Case studies and experiments," 2013 35th International Conference on Software Engineering (ICSE), San Francisco, CA, 2013, pp. 482-491.
doi: 10.1109/ICSE.2013.6606594
