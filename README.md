# SPL-FESG-Examples

In this repository, examples of product lines have been modelled by using Featured Event Sequence Graphs (FESG). A Featured ESG (FESG) is an extended ESG that is composed of a core ESG (c-ESG) and a set of feature ESGs (f-ESGs). The core of the product line represents the common behavior which exists in all products that belong to the product line. The core behavior is modelled using core ESG (c-ESG). An optional behavior is modelled using a feature ESG (f-ESG).

A Featured ESG is used in test sequence composition approach which composes the sequences of core and feature ESGs and generates a product's test sequences. This approach generates the event sequences of the core ESG and the feature ESGs and then, it composes these event sequences to generate a product configuration's event sequences. The sequences are composed thanks to the connection points i.e., (esgName,eventName) in the feature ESG(f-ESG) models' events.

To examine the examples and download the ESG files you can click the links below. The downloaded ESG models could be run on [Test Suite Designer](http://download.ivknet.de/) tool.

[Bank Account SPL](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/BankAccountProductLine.md) [1] \
[eMail SPL](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/EmailProductLine.md) [2] \
[Elevator SPL](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/ElevatorProductLine.md) [3] \
[Student Attendance System SPL](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/StudentAttendanceSystemSPL.md) [4] \
[Soda Vending Machine SPL](https://github.com/esg4aspl/SPL-FESG-Examples/blob/master/SodaVendingMachineSPL.md) [5]


## References

[1] Bank Account Product Line: http://spl2go.cs.ovgu.de/projects/54 (retrieved on 2022, April 23) \
[1] T. Thüm, I. Schaefer, S. Apel and M.Hentschel, "Family-Based Deductive Verification of Software Product Lines", 2012 Proceedings of the 11th International Conference on Generative Programming and Component Engineering, GPCE'12. 48. doi: 10.1145/2371401.2371404. \
[2] Email Product Line: http://spl2go.cs.ovgu.de/projects/17 (retrieved on 2022, April 23) \
[1,2] Thüm T, Schaefer I, Apel S, Hentschel M. Family-based deductive verification of software product lines. ACM SIGPLAN Notices 2012; 48: 11–20. doi: 10.1145/2480361.2371404. \
[1,2] Apel S, Speidel H, Wendler P, von Rhein A, Beyer D. Detection of feature interactions using feature-aware verification. In: ASE2011 International Conference on Automated Software Engineering; Lawrence, Kansas, USA; 2011. pp. 372–5. \
[1,2] Apel S, von Rhein A, Wendler P, Gro¨ßlinger A, Beyer D. Strategies for product-line verification: Case studies and experiments. In: ICSE 2013 International Conference on Software Engineering; San Francisco, CA, USA; 2013. pp.482–91. \
[3] Elevator Product Line: http://spl2go.cs.ovgu.de/projects/16 (retrieved on 2022, April 23) \
[4] http://www.splot-research.org/ (retrieved on 2022, April 23)\
[5] Classen A. Modelling and Model Checking Variability-Intensive Systems. PhD, University of Namur, Belgium, 2011.
