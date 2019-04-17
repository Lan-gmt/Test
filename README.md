Mã  nguồn  : bilibili/ijkplayer 
https://github.com/bilibili/ijkplayer/blob/master/android/ijkplayer/ijkplayer-java/src/main/java/tv/danmaku/ijk/media/player/IjkMediaMeta.java
Hàm  lựa chọn: 
public String getChannelLayoutInline() {					(1)
      if (mChannelLayout <= 0) {						(2)
            return "N/A";							(3)
      } else {									(4)
            if (mChannelLayout == AV_CH_LAYOUT_MONO) {				(5)
                return "mono";							(6)
            } else if (mChannelLayout == AV_CH_LAYOUT_STEREO) {			(7)
                return "stereo";						(8)
            } else {								(9)
                return String.format(Locale.US, "%x", mChannelLayout);		(10)
	}
}
Lập đồ thị:

 
Liệt kê các đường đi:
Đường 1:   1, 2, 3
Đường 2:   1, 2, 4, 5, 6
Đường 3:   1, 2, 4, 5, 7, 8
Đường 4:   1, 2, 4, 5, 7, 9, 10
Lập phương trình đường đi:
