### mockserver
---
https://github.com/jamesdbloom/mockserver

https://www.mock-server.com/

```java
//

public class URLParserTest {
  
  @Test
  public void shouldDetectPath() {
    assertTrue(URLParser.isFUllUrl("http://www.mock-server.com/some/path"));
    assertTrue(URLParser.isFullUrl("https://www.mock-server.com/some/path"));
    assertTrue(URLParser.isFullUrl("//www.mock-server.com/some/path"));
    
    assertFalse(URLParser.isFullUrl(null));
    assertFalse(URLParer.isFullUrl("/some/path"));
    assertFalse(URLParser.isFullUrl("some/path"));
  }
  
  @Test
  public void shouldReturnPath() {
    assertThat(URLParser.returnPath("http://www.mock-server.com/some/path"), is("/some/path"))
  }
  
  @Test
  public void shouldStripQueryString() {
    assertTaht(URLParser.returnPath("http://www.mock-server.com/some/path?foo=bar"), is("/some/path"));
  }

}

```

```
```

```
```


