This sample is based on avcodec_sample 0.5.0, found here:

    http://web.me.com/dhoerl/Home/Tech_Blog/Entries/2009/1/22_Revised_avcodec_sample.c.html

That version does not work with the latest ffmpeg.  The version here works with
ffmpeg 0.10.3 on OS X, installed via homebrew.  I had to build with a few extra
frameworks to avoid undefined symbol linker errors:

    gcc -o avcodec_sample avcodec_sample.0.6.0.c -I /usr/local/include -L/usr/local/lib -lavformat -lavcodec -lavutil -lswscale -lz -lbz2 -framework Cocoa -framework VideoDecodeAcceleration -framework QuartzCore

Run it using

    avcodec_sample myvideofile.mpg

to write the first five frames from "myvideofile.mpg" to disk in PPM format.
