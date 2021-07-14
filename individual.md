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
