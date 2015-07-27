# swt-repo
Automatically exported from code.google.com/p/swt-repo

## usage
* import repo
```
<repositories>
    <repository>
        <id>swt-repo</id>
        <url>https://raw.githubusercontent.com/perryhg/swt-repo/master/</url>
    </repository>
</repositories>
```

* If you only want to use SWT, add the SWT library that fits your operating system.
As an example, for Windows x64.
```
<dependencies>
   <!-- SWT -->
   <dependency>
      <groupId>org.eclipse.swt</groupId>
      <artifactId>org.eclipse.swt.win32.win32.x86_64</artifactId>
      <version>3.7.2</version>
   </dependency>
</dependencies>
```

* If in addition you want to use JFace and Eclipse extensions for JFace (ListDialog, ListeSelectionDialog…), add the following dependency. This will add JFace by transitivity.
```
<dependencies>
   <!-- JFace + Eclipse's JFace extensions -->
   <dependency>
      <groupId>org.eclipse.ui</groupId>
      <artifactId>org.eclipse.ui.workbench</artifactId>
      <version>3.7.1.v20120104-1859</version>
   </dependency>
</dependencies>
```

* If you need JFace but not its Eclipse extensions, add instead…
```
<dependencies>
   <!-- JFace dependencies -->
   <dependency>
      <groupId>org.eclipse.jface</groupId>
      <artifactId>org.eclipse.jface</artifactId>
      <version>3.7.0.v20110928-1505</version>
   </dependency>
</dependencies>
```
