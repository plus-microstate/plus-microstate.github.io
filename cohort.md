# The _microstate.cohort_ object

The _microstate.cohort_ object contains multiple data sets (e.g. multiple participants, scans, or trials in a task-based experiment), in contrast to the [microstate.individual](https://plus-microstate.github.io/individual) object which stores a single scan. In fact, the _microstate.cohort_ object contains a single _microstate.individual_ object per participant/trial/scan (hereon referred to as "individuals"), as well as information such as the condition of each individual and group-level microstate maps and statistics.

To create a _microstate.cohort_ object, type
```
coh = microstate.cohort
```
where `coh` is the _microstate.cohort_ object. Individuals can be added to this object using the methods under the **Importing/exporting data** section below. The methods listed below demonstrate options for preprocessing, analysing, and visualising the data at the group-level in +microstate.

### Properties

<table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Description</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <td>condition</td>
      <td>Array of integers labelling the condition corresponding to each individual</td>  
    </tr>
    <tr>
      <td>conditionlabels</td>
      <td>Cell array giving each integer value in cohort.condition a label</td> 
    </tr>
    <tr>
      <td>globalmaps</td>
      <td>Array of global microstate maps  </td> 
    </tr>
    <tr>
      <td>individual</td>
      <td>Array of microstate.individual objects representing each individual in the cohort </td>  
    </tr>      
    <tr>
      <td>process</td>
      <td>List of all processes performed on the data  </td>
    </tr>        
    <tr>
      <td>stats</td>
      <td>Structure containing group-level microstate statistics</td>  
    </tr>          
  </tbody>
</table>

### Methods

**Importing/exporting data**

<table>
  <thead>
    <tr>
      <th>Method</th>
      <th>Description</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <td>add_individuals</td>
      <td>Add an individual to the microstate.cohort object.  </td>  
    </tr>
    <tr>
      <td>delete_individuals</td>
      <td>Delete an individual from the microstate.cohort object. </td> 
    </tr>
  </tbody>
</table>

**Preprocessing data**

<table>
  <thead>
    <tr>
      <th>Method</th>
      <th>Description</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <td>ind_preprocess</td>
      <td>Run preprocess for each individual </td> 
    </tr>
    <tr>
      <td>ind_preprocess_ampenv</td>
      <td>Run preprocess_ampenv for each individual </td> 
    </tr>
    <tr>
      <td>ind_preprocess_filter</td>
      <td>Run preprocess_filter for each individual </td> 
    </tr>
    <tr>
      <td>ind_preprocess_orthogonalize</td>
      <td>Run preprocess_orthogonalize for each individual </td> 
    </tr>
    <tr>
      <td>ind_preprocess_rereference</td>
      <td>Run preprocess_rereference for each individual </td> 
    </tr>
    <tr>
      <td>ind_preprocess_resample</td>
      <td>Run preprocess_resample for each individual </td> 
    </tr>
    
  </tbody>
</table>

**Microstate analysis**

<table>
  <thead>
    <tr>
      <th>Method</th>
      <th>Description</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <td>cluster_global</td>
      <td>Perform group level microstate clustering </td> 
    </tr>
    <tr>
      <td>cluster_globalkoptimum</td>
      <td>Calculate optimum microstate maps at the group level.  </td> 
    </tr>
    <tr>
      <td>cluster_globalmaps2individual</td>
      <td>Align global maps to each individual   </td> 
    </tr>
    <tr>
      <td>ind_calculate_gfp</td>
      <td>Run calculate_gfp for each individual </td>
    </tr>
  </tbody>
</table>

**ERP/ERF analysis**

<table>
  <thead>
    <tr>
      <th>Method</th>
      <th>Description</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <td>erp_chi2stateprobs</td>
      <td>Perform chi2 test for responses and cluster permutation analysis </td>
    </tr>
    <tr>
      <td>erp_clusterperm_TANOVA</td>
      <td>Perform cluster permutation TANOVA analysis </td> 
    </tr>
    <tr>
      <td>erp_clusterperm_GFP</td>
      <td>Perform cluster permutation analysis on GFPs </td> 
    </tr>
    <tr>
      <td>erp_grandaverage</td>
      <td>	Calculate grand average ERPs  </td> 
    </tr>
  </tbody>
</table>


**Statistics and visualisation**

<table>
  <thead>
    <tr>
      <th>Method</th>
      <th>Description</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <td>cohort_stats</td>
      <td>Collect microstate statistics into a single structure</td>
    </tr>
    <tr>
      <td>ind_networks_wpli</td>
      <td>Run networks_wpli for each individual </td>
    </tr>
    <tr>
      <td>ind_stats_all</td>
      <td>Run stats_all for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_autoinformation</td>
      <td>Run stats_autoinformation for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_complexity</td>
      <td>Run stats_complexity for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_coverage</td>
      <td>Run stats_coverage for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_duration</td>
      <td>Run stats_duration for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_gev</td>
      <td>Run stats_gev for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_gfp_peaksfreq</td>
      <td>Run stats_gfp_peaksfreq for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_hurst</td>
      <td>Run stats_hurst for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_markov</td>
      <td>Run stats_markov for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_mututalinformation</td>
      <td>Run stats_mutualinformation for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_occurrence</td>
      <td>Run stats_occurrence for each individual </td> 
    </tr>
    <tr>
      <td>ind_stats_syntax</td>
      <td>Run stats_syntax for each individual </td> 
    </tr>
    <tr>
      <td>plot</td>
      <td>Visualise microstate data and statistics </td> 
    </tr>
    <tr>
      <td>stats_TANOVA</td>
      <td>Perform TANOVA analysis on clustered maps</td>
    </tr>
  </tbody>
</table>
