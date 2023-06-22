# SoundStream++ Audio Demo


## Abstract
In this paper, we propose SoundStream++, a high-rate extension of the SoundStream codec, which is able to generate almost transparent quality audio at 16 kbps for wideband speech signals. SoundStream shows reasonably good performance at low bit-rates (e.g. around 9 kbps), but its performance does not improve much when using more bits for encoding the latent embeddings. Motivated by experimental results showing that neural audio codec performance is highly related to the characteristics of latent embeddings such as dimensionality, dependency, and probability density function shape, we propose a convolutional transformer architecture and an attention-based multi-scale latent decomposition method that significantly enhances codec performance when quantizing high-dimensional embeddings. 
Experimental results show the superiority of our proposed model over conventional approaches.

## Audio Samples
Note: Encodec does not provide options for 9 kbps and 16 kbps.

### Bit-rate: 9 kbps
<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmoke; display: table;">
          <thead>
            <tr>
              <th style="width: 20%"></th>
              <th style="width: 20%">Opus</th>
              <th style="width: 20%">EVS (9.6kbps) </th>
              <th style="width: 20%">Encodec</th>
              <th style="width: 20%">SoundStream++</th>
            </tr>
          </thead>
          
          <tbody>
            <tr>
              <td style="width: 20%"><p>Sample 1</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/9kbps/file1-opus9.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/9kbps/file1-evs9-6.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/9kbps/file1-ss++9.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 2</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/9kbps/file2-opus9.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/9kbps/file2-evs-9-6.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/9kbps/file2-ss++9.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 3</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/9kbps/file3-opus9.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/9kbps/file3-evs9-6.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/9kbps/file3-ss++9.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>
            
            <tr>
              <td style="width: 20%"><p>Sample 4</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/9kbps/file4-opus9.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/9kbps/file4-evs9-6.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/9kbps/file4-ss++9.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>
          </tbody>
        </table>
    </div>
</div>

### Bit-rate: 12 kbps
<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmoke; display: table;">
          <thead>
            <tr>
              <th style="width: 20%"></th>
              <th style="width: 20%">Opus</th>
              <th style="width: 20%">EVS (13.2 kbps) </th>
              <th style="width: 20%">Encodec</th>
              <th style="width: 20%">SoundStream++</th>
            </tr>
          </thead>
          
          <tbody>
            <tr>
              <td style="width: 20%"><p>Sample 1</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/12kbps/file1-opus12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/12kbps/file1-evs-13-2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/12kbps/file1-encodec12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/12kbps/file1-ss++12.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 2</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/12kbps/file2-opus12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/12kbps/file2-evs-13-2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/12kbps/file2-encodec12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/12kbps/file2-ss++12.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 3</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/12kbps/file3-opus12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/12kbps/file3-evs-13-2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/12kbps/file3-encodec12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/12kbps/file3-ss++12.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 4</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/12kbps/file4-opus12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/12kbps/file4-evs-13-2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/12kbps/file4-encodec12.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/12kbps/file4-ss++12.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>          
    
          </tbody>
        </table>
    </div>
</div>

### Bit-rate: 16 kbps
<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmoke; display: table;">
          <thead>
            <tr>
              <th style="width: 20%"></th>
              <th style="width: 20%">Opus</th>
              <th style="width: 20%">EVS (16.4 kbps) </th>
              <th style="width: 20%">Encodec</th>
              <th style="width: 20%">SoundStream++</th>
            </tr>
          </thead>
          
          <tbody>
            <tr>
              <td style="width: 20%"><p>Sample 1</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/16kbps/file1-opus16.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/16kbps/file1-evs-16-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/16kbps/file1-ss++16.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 2</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/16kbps/file2-opus16.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/16kbps/file2-evs-16-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/16kbps/file2-ss++16.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 3</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/16kbps/file3-opus16.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/16kbps/file3-evs-16-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/16kbps/file3-ss++16.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 4</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/16kbps/file4-opus16.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/16kbps/file4-evs-16-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/16kbps/file4-ss++16.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

          </tbody>
        </table>
    </div>
</div>

### Bit-rate: 24 kbps
<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmoke; display: table;">
          <thead>
            <tr>
              <th style="width: 20%"></th>
              <th style="width: 20%">Opus</th>
              <th style="width: 20%">EVS (24.4 kbps) </th>
              <th style="width: 20%">Encodec</th>
              <th style="width: 20%">SoundStream++</th>
            </tr>
          </thead>
          
          <tbody>
            <tr>
              <td style="width: 20%"><p>Sample 1</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/24kbps/file1-opus24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/24kbps/file1-evs-24-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/24kbps/file1-encodec24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/24kbps/file1-ss++24.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 2</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/24kbps/file2-opus24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/24kbps/file2-evs-24-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/24kbps/file2-encodec24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/24kbps/file2-ss++24.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 3</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/24kbps/file3-opus24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/24kbps/file3-evs-24-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/24kbps/file3-encodec24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/24kbps/file3-ss++24.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 4</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/24kbps/file4-opus24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/24kbps/file4-evs-24-4.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/24kbps/file4-encodec24.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/24kbps/file4-ss++24.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

          </tbody>
        </table>
    </div>
</div>
