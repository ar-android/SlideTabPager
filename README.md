#Slide Tab Pager

This is xml

    <com.ocit.SlideTabPager
        android:id="@+id/tabs"
        android:layout_width="match_parent"
        android:layout_height="48dp"
        app:pstsShouldExpand="true"
        app:pstsTextAllCaps="true" >
    </com.ocit.SlideTabPager>


This is to aplly library

SlideTabPager tabsStrip = (SlideTabPager) findViewById(R.id.tabs);
tabsStrip.setViewPager(viewPager);


