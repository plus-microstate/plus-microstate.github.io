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
      <td>define_trials</td>
      <td>Segment a single dataset into trials based on either a fixed length or stimulus times. </td> 
    </tr>
    <tr>
    <td>preprocess</td>
      <td>Wrapper for a default preprocessing pipeline. </td> 
    </tr>
    <td>preprocess_ampenv</td>
      <td>Calculate amplitude envelope of data. </td> 
    </tr>
    <td>preprocess_filter</td>
      <td>Bandpass or bandstop filter data. </td> 
    </tr>
    <td>preprocess_orthogonalize</td>
      <td>Orthogonalize time courses. </td> 
    </tr>
    <td>preprocess_rereference</td>
      <td>Re-reference data to average (EEG only). </td> 
    </tr>
    <td>preprocess_resample</td>
      <td>Resample data. </td> 
    </tr>
    
  </tbody>
</table>
