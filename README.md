# Light Semantic Data Transformations 
*"If in doubt, leave it out".*

Semantic data transformations & especially hidden semantic data transformations
are everywhere.

# The key idea # 
They key idea of light semantic data transformation is 
- that you should separate business/"semantic" logic data transformations like renaming things, 
deducing things from analytical data transformations like aggregating, grouping, counting,...
- that this is extremely hard because of a lot of "hidden semantic transformations", assumptions you're making on
interfaces which usually are not as fixed as you might like
- that you therefore simply separate them and try to mostly leave out the business & "semantic" data transformations.
- and test the hell out of your "hidden" assumptions right at the start.

## What's in here ##
- [A light introduction to light data transformations](Tranformations_Light.ipynb)
- [One short example of light transformations applied](Applied 1.ipynb)

## WIP Next Up ##
- Hidden Transformations like importing XMLs from a string column, assumptions
on the length of strings, uniqueness of "ids"
- Testing & Assumptions. Where do we test assumptions? Close to the source.
After that we do not test for "uniqueness" but rather our transformation logic...
(Or do we? Kinda yes, because of assumptions...) We may combine both, but
not 1 without the other! (So uniqueness on front model is fine, if 
  I have uniqueness in source!)
- "reason for X; making complexer things apparent"
- "hidden domain knowledge => without fixed interfaces always somewhere..."
