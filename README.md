#Slide Tab Pager

# Usage
```
    <com.ocit.SlideTabPager
        android:id="@+id/tabs"
        android:layout_width="match_parent"
        android:layout_height="48dp"
        app:pstsShouldExpand="true"
        app:pstsTextAllCaps="true" >
    </com.ocit.SlideTabPager>
```

  In your `onCreate` method (or `onCreateView` for a fragment), bind the
  widget to the `ViewPager`.

        // Initialize the ViewPager and set an adapter
	ViewPager viewPager = (ViewPager) findViewById(R.id.viewpager);
	viewPager.setAdapter(new PagerAdapter(getSupportFragmentManager()));
	
         // Bind the tabs to the ViewPager
	SlideTabPager tabsStrip = (SlideTabPager) findViewById(R.id.tabs);
	tabsStrip.setViewPager(viewPager);

  *(Optional)* If you use an `OnPageChangeListener` with your view pager
  you should set it in the widget rather than on the pager directly.

         // continued from above
         tabs.setOnPageChangeListener(mPageChangeListener);


