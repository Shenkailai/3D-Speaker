add_executable(read_and_describe_wav read_and_describe_wav.cpp)
target_link_libraries(read_and_describe_wav utils)

add_executable(make_fbank_feature make_fbank_feature.cpp)
target_link_libraries(make_fbank_feature PUBLIC utils feature)

add_executable(extract_speaker_embedding extract_speaker_embedding.cpp)
target_link_libraries(extract_speaker_embedding PUBLIC utils feature model)
