# SoundStream++ Audio Demo


## Abstract
In this paper, we propose SoundStream++, a high-rate extension of the SoundStream codec, which is able to generate almost transparent quality audio at 16 kbps for wideband speech signals. SoundStream shows reasonably good performance at low bit-rates (e.g. around 9 kbps), but its performance does not improve much when using more bits for encoding the latent embeddings. Motivated by experimental results showing that neural audio codec performance is highly related to the characteristics of latent embeddings such as dimensionality, dependency, and probability density function shape, we propose a convolutional transformer architecture and an attention-based multi-scale latent decomposition method that significantly enhances codec performance when quantizing high-dimensional embeddings. 
Experimental results show the superiority of our proposed model over conventional approaches.

## Audio Samples

### Bit-rate: 9 kbps
<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmoke; display: table;">
          <thead>
            <tr>
              <th style="width: 20%"></th>
              <th style="width: 20%">Opus</th>
              <th style="width: 20%">EVS</th>
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
                    <source src="Opus/9kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/9kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/9kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/9kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 2</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/9kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/9kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/9kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/9kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 3</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/9kbps/sample3.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/9kbps/sample3.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/9kbps/sample3.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/9kbps/sample3.wav" type="audio/wav" />
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
              <th style="width: 20%">EVS</th>
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
                    <source src="Opus/12kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/12kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/12kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/12kbps/sample1.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 2</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/12kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/12kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/12kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/12kbps/sample2.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td style="width: 20%"><p>Sample 3</p>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Opus/12kbps/sample3.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="EVS/12kbps/sample3.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="Encodec/12kbps/sample3.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 20%">
                <audio id="player" controls style="width: 100%;">
                    <source src="SoundStream++/12kbps/sample3.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>
          </tbody>
        </table>
    </div>
</div>
