# software_default_predictions

Source:- http://promise.site.uottawa.ca/SERepository/datasets/jm1.arff

The dataset is taken from Promise site.

1. Title/Topic: JM1/software defect prediction
 
% 2. Sources:
% 
%    -- Creators:  NASA, then the NASA Metrics Data Program,
%       -- http://mdp.ivv.nasa.gov. Contacts: Mike Chapman, 
%          Galaxy Global Corporation (Robert.Chapman@ivv.nasa.gov)
%          +1-304-367-8341; Pat Callis, NASA, NASA project manager 
%          for MDP (Patrick.E.Callis@ivv.nasa.gov) +1-304-367-8309 
% 
%    -- Donor: Tim Menzies (tim@barmag.net)
% 
%    -- Date:  December 2 2004

 -- JM1 is written in "C" and is a real-time predictive ground system: 
%        Uses simulations to generate predictions
%
%    -- Data comes from McCabe and Halstead features extractors of
%    source code.  These features were defined in the 70s in an attempt
%    to objectively characterize code features that are associated with
%    software quality.  The nature of association is under dispute.
%    Notes on McCabe and Halstead follow.
%    
%    -- The McCabe and Halstead measures are "module"-based where a
%    "module" is the smallest unit of functionality. In C or Smalltalk,
%    "modules" would be called "function" or "method" respectively.

Attribute Information:
% 	
%      1. loc             : numeric % McCabe's line count of code
%      2. v(g)            : numeric % McCabe "cyclomatic complexity"
%      3. ev(g)           : numeric % McCabe "essential complexity"
%      4. iv(g)           : numeric % McCabe "design complexity"
%      5. n               : numeric % Halstead total operators + operands
%      6. v               : numeric % Halstead "volume"
%      7. l               : numeric % Halstead "program length"
%      8. d               : numeric % Halstead "difficulty"
%      9. i               : numeric % Halstead "intelligence"
%     10. e               : numeric % Halstead "effort"
%     11. b               : numeric % Halstead 
%     12. t               : numeric % Halstead's time estimator
%     13. lOCode          : numeric % Halstead's line count
%     14. lOComment       : numeric % Halstead's count of lines of comments
%     15. lOBlank         : numeric % Halstead's count of blank lines
%     16. lOCodeAndComment: numeric
%     17. uniq_Op         : numeric % unique operators
%     18. uniq_Opnd       : numeric % unique operands
%     19. total_Op        : numeric % total operators
%     20. total_Opnd      : numeric % total operands
%     21: branchCount     : numeric % of the flow graph
%     22. defects         : {false,true} % module has/has not one or more 
%                                        % reported defects


AIM: - Performe EDA on dataset and look for distribution.
       Handle Missing values.
       Handle imbalance in dataset.
       Scaling the dataset.
       Applying Multiple machine learning algorithams which are robust to outliers and check the accuracy.
       Hyperparameter tune the model that pperforms good.
%
