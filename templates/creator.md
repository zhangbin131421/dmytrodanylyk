![Creator](/assets/images/templates/creator.gif)

Name | Expression | Default Value | Skip if defined
--- | --- | --- | ---
TYPE | className() | Object | true

```java
public static final Parcelable.Creator<$TYPE$> CREATOR = new Parcelable.Creator<$TYPE$>() {
    
    @Override
    public $TYPE$ createFromParcel(Parcel in) {
        return new $TYPE$(in);
    }

    @Override
    public $TYPE$[] newArray(int size) {
        return new $TYPE$[size];
    }
};

public $TYPE$(Parcel parcel) {
  // parcel.readInt();
}
```
