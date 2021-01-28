Django does not serve static files like css, javascript, and images by deagult 

``` 
from django.conf import settings
from django.conf.urls.static import static

urlpatterns += static(settings.STATIC_URL, document_root=settings.STATIC_ROOT)
````