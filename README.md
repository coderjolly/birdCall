# Bird Species Classification Using Bird Call Recordings
There are already many projects underway to extensively monitor birds by continuously recording natural soundscapes over long periods. However, as many living and nonliving things make noise, the analysis of these datasets is often done manually by domain experts. These analyses are painstakingly slow, and results are often incomplete. Data science may be able to assist, so researchers have turned to large crowd sourced databases of focal recordings of birds to train AI models. Unfortunately, there is a domain mismatch between the training data (short recording of individual birds) and the soundscape recordings (long recordings with often multiple species calling at the same time) used in monitoring applications. This is one of the reasons why the performance of the currently used AI models has been subpar. To unlock the full potential of these extensive and information-rich sound archives, researchers need good machine listeners to reliably extract as much information as possible to aid data-driven conservation.

# Directory Structure

-  **[1_audio_data](https://github.com/teambirdcall/birdcall/tree/main/1_audio_data)** - Contains the raw Audio files categorized by their species name as folders. This folder should contain the original audios that have not been chunked and are of variable length.

-  **[2_denoise_data](https://github.com/teambirdcall/birdcall/tree/main/2_denoise_data)** - Contains the denoised raw Audio files categorized by their species name as folders.

-  **[3_chunk_data](https://github.com/teambirdcall/birdcall/tree/main/3_chunk_data)** - It contains the chunked audios as per respective species folder that have been made from audiodata folder.

-  **[4_pitch_change](https://github.com/teambirdcall/birdcall/tree/main/4_pitch_change)** - It contains the pickle files of each respective species that have changed on the basis of pitch and dumped in this folder.

-  **[5_time_change](https://github.com/teambirdcall/birdcall/tree/main/5_time_change)** - It contains the pickle files of each respective species that have changed on the basis of time and dumped in this folder.

-  **[6_mel_result](https://github.com/teambirdcall/birdcall/tree/main/6_mel_result)**- It contains the mel-spectrogram of chunked audios as per respective species that have been made from result folder.

-  **[7_mfcc_result](https://github.com/teambirdcall/birdcall/tree/main/7_mfcc_result)** - It contains the mfcc-data in the form of pickle files of all the species in the result folder.