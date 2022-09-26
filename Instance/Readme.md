Sumber Dataset:
## How to cite the article journal
Michelini, A., Cianetti, S., Gaviano, S., Giunchi, C., Jozinović, D., and Lauciani, V., INSTANCE – the Italian seismic dataset for machine learning, Earth Syst. Sci. Data, 13 (12), 5509 – 5544, [doi:10.5194/essd-13-5509-2021](https://essd.copernicus.org/articles/13/5509/2021/).

## How to cite the dataset
**INSTANCE** The Italian Seismic Dataset For Machine Learning,
Alberto Michelini, Spina Cianetti, Sonja Gaviano, Carlo Giunchi, Dario Jozinović & Valentino Lauciani,
Seismic Waveforms And Associated Metadata published 2021 in Istituto Nazionale di Geofisica e Vulcanologia (INGV) https://doi.org/10.13127/instance

## Downloads
To get the **full INSTANCE dataset** you have to download:

* **Events metadata version 2** ([**csv**](http://repo.pi.ingv.it/instance/metadata_Instance_events_v2.csv.bz2), 238 MB bz2 file, 1.1 GB after decompression, doi:10.13127/instance/eventsmetadata.2). Fixed the metadata parameter name source_mt_scalar_moment_Nm.
* **Events metadata version 1** ([**csv**](http://repo.pi.ingv.it/instance/metadata_Instance_events.csv.bz2), 238 MB bz2 file, 1.1 GB after decompression, doi:10.13127/instance/eventsmetadata.1)
* **Events data in counts**  as [**single hdf5 file**](http://repo.pi.ingv.it/instance/Instance_events_counts.hdf5.bz2) (39 GB bz2 file, 156 GB after decompression) or 10 GB parts ([**part-a**](http://repo.pi.ingv.it/instance/events/Instance_events_counts.hdf5.bz2.part-a), [**part-b**](http://repo.pi.ingv.it/instance/events/Instance_events_counts.hdf5.bz2.part-b), [**part-c**](http://repo.pi.ingv.it/instance/events/Instance_events_counts.hdf5.bz2.part-c), [**part-d**](http://repo.pi.ingv.it/instance/events/Instance_events_counts.hdf5.bz2.part-d), doi:10.13127/instance/events.1)

* **Events data in ground motion units** as [**single hdf5 file**](http://repo.pi.ingv.it/instance/Instance_events_gm.hdf5.bz2) (151 GB bz2 file, 156 GB after decompression) or
20 GB parts ([**part-a**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-a),
[**part-b**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-b),
[**part-c**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-c),
[**part-d**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-d),
[**part-e**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-e),
[**part-f**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-f),
[**part-g**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-g),
[**part-h**](http://repo.pi.ingv.it/instance/gm/Instance_events_gm.hdf5.bz2.part-h)). Ground motion units are m/s for HH and EH channels and m/s<sup>2</sup> for HN channel, doi:10.13127/instance/groundmotion.1
* **Noise metadata** ([**csv**](http://repo.pi.ingv.it/instance/metadata_Instance_noise.csv.bz2), 6.7 MB bz2 file, 53 MB after decompression, doi:10.13127/instance/noisemetadata.1)
* **Noise data** in counts ([**hdf5**](http://repo.pi.ingv.it/instance/Instance_noise.hdf5.bz2), 3.9 GB bz2 file, 18 GB after decompression, doi:10.13127/instance/noise.1)


* **Stations inventory** ([**StationXML**](http://repo.pi.ingv.it/instance/responses.tgz), 15 MB)

<!-- The **notebooks** provided in this repo can be used to reproduce the figures of the manuscript Michelini et al., 2021, submitted. -->
All the above downloads provide `bzip2` compressed files. The multipart files can be reassembled and then unzipped (e.g., for the event data file)

```
cat  Instance_events_counts.hdf5.bz2.part-* > Instance_events_counts.hdf5.bz2
bzip2 -d Instance_events_counts.hdf5.bz2
```

A **sample dataset** of about 1.7 GB is provided to run the notebooks. This contains 10,000 events and 1000 noise waveforms together with the associated metadata. Potentially interested users can evaluate **INSTANCE**  data and metadata without downloading the whole dataset.

* [**Sample dataset vesrion 2**](http://repo.pi.ingv.it/instance/Instance_sample_dataset_v2.tar.bz2) (1.7 GB bz2 file, 2.74 GB after decompression). Fixed the metadata parameter name source_mt_scalar_moment_Nm.
* [**Sample dataset version 1**](http://repo.pi.ingv.it/instance/Instance_sample_dataset.tar.bz2) (1.7 GB bz2 file, 2.74 GB after decompression)

