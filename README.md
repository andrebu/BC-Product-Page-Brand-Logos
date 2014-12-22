BigCommerce-Product-Page-Brand-Logos
====================================

BigCommerce Product Page Brand Logos which appear to the right, in the Product details section.  These logos will be dynamically pulled from the brand's respective brand page.

```HTML
                   <script type="text/javascript">    
                        $(document).ready(function() {
            
                            $.ajax({
                              url: "http://andredevelopment.mybigcommerce.com/brands/" 
            
                            }).done(function ( data ) {
                                var html = $(data);
                                var items = $('.SubBrandListGrid li', html);
            
                                items.each(function() {
                                    var link = $('a', this);
                                    if(link){
                                    var txt = $(link).text();   
                                    var brname = '%%GLOBAL_BrandName%%'
                                    var replaced1 = txt.trim();                             
                                    var replaced2 = String(brname.replace(/ /g, ' '));     
                                        if( replaced1 === replaced2 ){
                                            var img = $('img', this).attr('src');
                                            $('#brand-logo').attr('src', img);
                                        }        
                                    }                                
                                });                             
                            });
                        });
                    </script>
```


=========================================================================================================
=========================================================================================================
=========================================================================================================



10.   Dynamic brand Logos

                    <script type="text/javascript">    
                        $(document).ready(function() {
            
                            $.ajax({
                              url: "http://andredevelopment.mybigcommerce.com/brands/" 
            
                            }).done(function ( data ) {
                                var html = $(data);
                                var items = $('.SubBrandListGrid li', html);
            
                                items.each(function() {
                                    var link = $('a', this);
                                    if(link){
                                    var txt = $(link).text();   
                                    var brname = '%%GLOBAL_BrandName%%'
                                    var replaced1 = txt.trim();                             
                                    var replaced2 = String(brname.replace(/ /g, ' '));     
                                        if( replaced1 === replaced2 ){
                                            var img = $('img', this).attr('src');
                                            $('#brand-logo').attr('src', img);
                                        }        
                                    }                                
                                });                             
                            });
                        });
                    </script>



				
<h1><img src="/templates/__custom/images/BrandDefault.gif" border="0" id="brand-logo">  
    %%GLOBAL_TrailBrandName%%                         
	                    <script type="text/javascript">    
                        $(document).ready(function() {
            
                            $.ajax({
                              url: "http://andredevelopment.mybigcommerce.com/brands/" 
            
                            }).done(function ( data ) {
                                var html = $(data);
                                var items = $('.SubBrandListGrid li', html);
            
                                items.each(function() {
                                    var link = $('a', this);
                                    if(link){
                                    var txt = $(link).text();   
                                    var brname = '%%GLOBAL_TrailBrandName%%'
                                    var replaced1 = txt.trim();                             
                                    var replaced2 = String(brname.replace(/ /g, ' '));     
                                        if( replaced1 === replaced2 ){
                                            var img = $('img', this).attr('src');
                                            $('#brand-logo').attr('src', img);
                                        }        
                                    }                                
                                });                             
                            });
                        });
                    </script>
</h1>
	
