# The _microstate.individual_ object

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
      <td>bad_samples</td>
      <td>Array specifying which samples are bad samples (e.g. artifacts)</td>  
    </tr>
    <tr>
      <td>data</td>
      <td>Number of samples x number of channels (or ROIs) array of MEG/EEG/source/amplitude envelope time courses</td> 
    </tr>
    <tr>
      <td>gfp</td>
      <td>1 x Number of samples array containing the GFP values </td> 
    </tr>
    <tr>
      <td>label</td>
      <td>1 x number of samples array containing microstate labels of each sample</td>  
    </tr>  
    <tr>
      <td>maps</td>
      <td>Number of channels (or ROIs) x number of microstates array containing microstate maps</td>  
    </tr>
    <tr>
      <td>modality</td>
      <td>Character array, either 'eeg', 'meg', 'source', or 'ampenv'</td>  
    </tr>      
    <tr>
      <td>process</td>
      <td>Table listing every process performed on data</td>
    </tr>
    <tr>
      <td>sample</td>
      <td>1 x number of samples array specifying which samples are included from the original dataset</td>
    </tr>          
    <tr>
      <td>stats</td>
      <td>Structure containing microstate statistics</td>  
    </tr>          
    <tr>
      <td>time</td>
      <td>1 x number of samples array containing the time axis</td>
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
      <td>add_data</td>
      <td>Add data to empty microstate.individual object. </td>  
    </tr>
    <tr>
      <td>export_struct</td>
      <td>Export microstate.individual object's properties to a MATLAB structure.</td> 
    </tr>
    <tr>
      <td>import_brainstorm</td>
      <td>Function to import brainstorm source data. </td>  
    </tr>  
    <tr>
      <td>import_eeglab</td>
      <td>Function to import data from EEGLab. </td>  
    </tr>
    <tr>
      <td>import_fieldtrip</td>
      <td>Function to import data from Fieldtrip. </td>  
    </tr>      
    <tr>
      <td>import_loreta</td>
      <td>Function to import source reconstructions from LORETA or sLORETA/eLORETA software</td>
    </tr>
    <tr>
      <td>import_spm_meeg</td>
      <td>Function to import SPM M/EEG objects.</td>
    </tr>          
    <tr>
      <td>import_spm_nifti</td>
      <td>Function to import NiFTi images.</td>  
    </tr>          
    <tr>
      <td>import_struct</td>
      <td>Imports data saved using individual.export_struct.</td>
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
      <td>add_bad_samples</td>
      <td>Specify bad samples in microstate.individual object. </td>
    </tr>
    <tr>
      <td>define_trials</td>
      <td>Segment a single dataset into trials based on either a fixed length or stimulus times. </td> 
    </tr>
    <tr>
      <td>preprocess</td>
      <td>Wrapper for a default preprocessing pipeline. </td> 
    </tr>
    <tr>
      <td>preprocess_ampenv</td>
      <td>Calculate amplitude envelope of data. </td> 
    </tr>
    <tr>
      <td>preprocess_filter</td>
      <td>Bandpass or bandstop filter data. </td> 
    </tr>
    <tr>
      <td>preprocess_orthogonalize</td>
      <td>Orthogonalize time courses. </td> 
    </tr>
    <tr>
      <td>preprocess_rereference</td>
      <td>Re-reference data to average (EEG only). </td> 
    </tr>
    <tr>
      <td>preprocess_resample</td>
      <td>Resample data. </td> 
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
      <td>calculate_gfp</td>
      <td>Calculate GFP of time series  </td>
    <tr>
      <td>cluster_alignmaps</td>
      <td>Assign a microstate class to each time point, building a discrete microstate time series. </td> 
    </tr>
    <tr>
    <td>cluster_estimatemaps</td>
      <td>Cluster to calculate a specified number of microstate maps </td> 
    </tr>
    <td>cluster_get_gfppeaks</td>
      <td>Extract GFP peaks of the data.  </td> 
    </tr>
    <td>cluster_koptimum</td>
      <td>Calculate optimum number of microstate classes </td> 
    </tr>
    <td>cluster_label2maps</td>
      <td>Calculate centroid maps given data and microstate labels  </td>     
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
      <td>networks_wpli</td>
      <td>Calculate microstate segmented functional connectivity </td>
    <tr>
      <td>plot</td>
      <td>Visualise properties of the data and microstates </td> 
    </tr>
    <tr>
    <td>stats_all</td>
      <td>Calculate all microstate statistics </td> 
    </tr>
    <td>stats_autoinformation</td>
      <td>Calculate autoinformation of microstate sequence  </td> 
    </tr>
    <td>stats_complexity</td>
      <td>Calculate microstate transition complexity </td> 
    </tr>
    <tr>
    <td>stats_coverage</td>
      <td>Calculate coverage of microstates </td> 
    </tr>
    <tr>
    <td>stats_duration</td>
      <td>Calculate durations of microstates </td> 
    </tr>
    <tr>
    <td>stats_gev</td>
      <td>Calculate GEV of microstates </td> 
    </tr>
    <tr>
    <td>stats_gfp_peaksfreq</td>
      <td>Calculate number of GFP peaks per second </td> 
    </tr>
    <tr>
    <td>stats_hurst</td>
      <td>Calculate Hurst exponent of microstate sequences </td> 
    </tr>
    <tr>
    <td>stats_markov</td>
      <td>Calculate Markov matrix and Markov statistics </td> 
    </tr>
    <tr>
    <td>stats_mututalinformation</td>
      <td>Calculate mutual information between microstate sequence and another sequence (2nd input) </td> 
    </tr>
    <tr>
    <td>stats_occurrence</td>
      <td>Calculate number of occurrences of a microstate per second </td> 
    </tr>
    <tr>
    <td>stats_syntax</td>
      <td>Calculate syntax matrix </td> 
    </tr>
  </tbody>
</table>
