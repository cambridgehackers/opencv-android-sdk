opencv-android-sdk
==================

Build of opencv-android-sdk

Built as follows:
OPENCV_DIR=$PWD

mkdir build; cd build

cmake -DCMAKE_TOOLCHAIN_FILE=$OPENCV_DIR/platforms/android/android.toolchain.cmake -DANDROID_STL=stlport_static -DANDROID_NATIVE_API_LEVEL=19 ..
make -j8
make install
