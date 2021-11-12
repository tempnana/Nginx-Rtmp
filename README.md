# Nginx
Nginx Install
<br>
<pre>
bash <(wget -qO- https://raw.githubusercontent.com/tempnana/Nginx/main/install.sh)
</pre>
<br>
<code>/etc/nginx/nginx.conf</code>
<br>
<code>/etc/nginx/vhost/</code>
<br>
<code>/etc/nginx/html/</code>
<br>
<code>/usr/lib/nginx/modules/</code>
<br>
<code>/var/log/nginx/access.log</code>
<br>
<code>/var/log/nginx/error.log</code>
<br>
<br>
<pre>service nginx (restart|reload|start|status|stop)</pre>
<br>
<br>
<pre>
./configure --prefix=/etc/nginx \
            --sbin-path=/usr/sbin/nginx \
	    --modules-path=/usr/lib/nginx/modules \
	    --conf-path=/etc/nginx/nginx.conf \
	    --error-log-path=/var/log/nginx/error.log \
	    --http-log-path=/var/log/nginx/access.log \
	    --pid-path=/var/run/nginx.pid \
	    --lock-path=/var/run/nginx.lock \
	    --http-client-body-temp-path=/var/cache/nginx/client_temp \
	    --http-proxy-temp-path=/var/cache/nginx/proxy_temp \
	    --http-fastcgi-temp-path=/var/cache/nginx/fastcgi_temp \
	    --http-uwsgi-temp-path=/var/cache/nginx/uwsgi_temp \
	    --http-scgi-temp-path=/var/cache/nginx/scgi_temp \
	    --user=nginx \
	    --group=nginx \
	    --with-compat \
	    --with-file-aio \
	    --with-threads \
	    --with-http_addition_module \
	    --with-http_auth_request_module \
	    --with-http_dav_module \
	    --with-http_flv_module \
	    --with-http_gunzip_module \
	    --with-http_gzip_static_module \
	    --with-http_mp4_module \
	    --with-http_random_index_module \
	    --with-http_realip_module \
	    --with-http_secure_link_module \
	    --with-http_slice_module \
	    --with-http_ssl_module \
	    --with-http_stub_status_module \
	    --with-http_sub_module \
	    --with-http_v2_module \
	    --with-mail \
	    --with-mail_ssl_module \
	    --with-stream \
	    --with-stream_realip_module \
	    --with-stream_ssl_module \
	    --with-stream_ssl_preread_module \	
	    --with-pcre=../pcre-8.43 \
	    --with-pcre-jit \
            --with-zlib=../zlib-1.2.11 \
	    --with-openssl=../openssl-1.1.1d \
	    --with-openssl-opt=no-nextprotoneg \			
	    --with-debug \			
	    --with-ngx_cache_purge \		
	    --with-ngx_http_substitutions
</pre>
