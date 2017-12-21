+++
# Type of content, set "slide" to display it fullscreen with reveal.js
type="page"
title = "Request Won't Show"
description = "OPRA request won't show"
date = "2017-12-19T18:36:24+02:00"
# Creator's Display name
creatordisplayname = "Gavin Rozzi"
# Creator's Email
creatoremail = "gr@gavinrozzi.com"
# LastModifier's Display name
lastmodifierdisplayname = "Gavin Rozzi"
# LastModifier's Email
lastmodifieremail = "gr@gavinrozzi.com"
+++

One OPRA response simply will not show, no matter what we try and do. This is a mystery and we have not been sure how to proceed.

## Upstream Github issue
We have opened a [Github issue](https://github.com/mysociety/alaveteli/issues/4412) with the open source software project that provides the code that runs on the OPRAmachine server. We are curently waiting to hear back as of 12/20/2017.

## Full Error message

A RuntimeError occurred in request#show:

 main body text more than 1 MB, need to implement clipping like for attachment text, or there is some other MIME decoding problem or similar
 app/models/incoming_message.rb:426:in `_cache_main_body_text'


-------------------------------
Request:
-------------------------------

 * URL        : https://opramachine.com/request/opra_requests_5
 * HTTP Method: GET
 * IP address : 157.55.39.120
 * Parameters : {"controller"=>"request", "action"=>"show", "url_title"=>"opra_requests_5"}
 * Timestamp  : 2017-12-20 23:22:06 -0500
 * Server : opramachine.com
 * Rails root : /var/www/opramachine.com/alaveteli
 * Process: 23591

-------------------------------
Session:
-------------------------------

 * session id: [FILTERED]
 * data: {"session_id"=>"6748e0b4f9d0d1600d1fcd55aa207611", "locale"=>"en"}

-------------------------------
Environment:
-------------------------------

 * GATEWAY_INTERFACE                              : CGI/1.2
 * HTTP_ACCEPT                                    : */*
 * HTTP_ACCEPT_ENCODING                           : gzip, deflate
 * HTTP_CACHE_CONTROL                             : no-cache
 * HTTP_CONNECTION                                : close
 * HTTP_FROM                                      : bingbot(at)microsoft.com
 * HTTP_HOST                                      : opramachine.com
 * HTTP_PRAGMA                                    : no-cache
 * HTTP_USER_AGENT                                : Mozilla/5.0 (compatible; bingbot/2.0; +http://www.bing.com/bingbot.htm)
 * HTTP_VERSION                                   : HTTP/1.0
 * HTTP_X_ACCEL_MAPPING                           : /var/www/opramachine.com/alaveteli/cache/zips/production/download=/download
 * HTTP_X_FORWARDED_FOR                           : 157.55.39.120
 * HTTP_X_FORWARDED_PROTO                         : https
 * HTTP_X_REAL_IP                                 : 157.55.39.120
 * HTTP_X_SENDFILE_TYPE                           : X-Accel-Redirect
 * ORIGINAL_FULLPATH                              : /request/opra_requests_5
 * ORIGINAL_SCRIPT_NAME                           :
 * PATH_INFO                                      : /request/opra_requests_5
 * QUERY_STRING                                   :
 * REMOTE_ADDR                                    : 127.0.0.1
 * REQUEST_METHOD                                 : GET
 * REQUEST_PATH                                   : /request/opra_requests_5
 * REQUEST_URI                                    : /request/opra_requests_5
 * ROUTES_53640860_SCRIPT_NAME                    :
 * SCRIPT_NAME                                    :
 * SERVER_NAME                                    : opramachine.com
 * SERVER_PORT                                    : 80
 * SERVER_PROTOCOL                                : HTTP/1.1
 * SERVER_SOFTWARE                                : thin 1.5.1 codename Straight Razor
 * action_controller.instance                     : #<RequestController:0x000000102f2640>
 * action_dispatch.backtrace_cleaner              : #<Rails::BacktraceCleaner:0x0000000a89b570>
 * action_dispatch.cookies                        : #<ActionDispatch::Cookies::CookieJar:0x00000010393180>
 * action_dispatch.cookies_digest                 :
 * action_dispatch.cookies_serializer             : hybrid
 * action_dispatch.encrypted_cookie_salt          : encrypted cookie
 * action_dispatch.encrypted_signed_cookie_salt   : signed encrypted cookie
 * action_dispatch.http_auth_salt                 : http authentication
 * action_dispatch.key_generator                  : #<ActiveSupport::CachingKeyGenerator:0x000000095c7368>
 * action_dispatch.logger                         : #<ActiveSupport::Logger:0x0000000655fa18>
 * action_dispatch.parameter_filter               : [:password]
 * action_dispatch.redirect_filter                : []
 * action_dispatch.remote_ip                      : 157.55.39.120
 * action_dispatch.request.accepts                : [#<Mime::Type:0x000000102f0ca0 @synonyms=[], @symbol=nil, @string="*/*", @hash=4306184708532017714>]
 * action_dispatch.request.content_type           :
 * action_dispatch.request.flash_hash             : #<ActionDispatch::Flash::FlashHash:0x0000001145a4c8>
 * action_dispatch.request.formats                : [#<Mime::Type:0x000000102f0ca0 @synonyms=[], @symbol=nil, @string="*/*", @hash=4306184708532017714>]
 * action_dispatch.request.parameters             : {"controller"=>"request", "action"=>"show", "url_title"=>"opra_requests_5"}
 * action_dispatch.request.path_parameters        : {:controller=>"request", :action=>"show", :url_title=>"opra_requests_5"}
 * action_dispatch.request.query_parameters       : {}
 * action_dispatch.request.request_parameters     : {}
 * action_dispatch.request.unsigned_session_cookie: {"session_id"=>"6748e0b4f9d0d1600d1fcd55aa207611"}
 * action_dispatch.request_id                     : 9e9248e2-8440-457b-87b4-d8568a9ca412
 * action_dispatch.routes                         : #<ActionDispatch::Routing::RouteSet:0x0000000664fd38>
 * action_dispatch.secret_key_base                : this default is insecure as code is open source, please override for live sites in config/general; this will do for local development
 * action_dispatch.secret_token                   :
 * action_dispatch.show_detailed_exceptions       : false
 * action_dispatch.show_exceptions                : true
 * action_dispatch.signed_cookie_salt             : signed cookie
 * async.callback                                 : #<Method: Thin::Connection#post_process>
 * async.close                                    : #<EventMachine::DefaultDeferrable:0x000000102ccc10>
 * newrelic.transaction_started                   : true
 * rack.errors                                    : #<IO:0x00000002041b98>
 * rack.input                                     : #<StringIO:0x000000102cd520>
 * rack.multiprocess                              : false
 * rack.multithread                               : false
 * rack.request.cookie_hash                       : {}
 * rack.request.query_hash                        : {}
 * rack.request.query_string                      :
 * rack.run_once                                  : false
 * rack.session                                   : #<ActionDispatch::Request::Session:0x000000102ec5b0>
 * rack.session.options                           : #<ActionDispatch::Request::Session::Options:0x000000102ec560>
 * rack.url_scheme                                : http
 * rack.version                                   : [1, 0]

-------------------------------
Backtrace:
-------------------------------

 app/models/incoming_message.rb:426:in `_cache_main_body_text'
 app/models/incoming_message.rb:452:in `get_main_body_text_unfolded'
 app/models/incoming_message.rb:616:in `get_body_for_html_display'
 app/views/request/_incoming_correspondence.html.erb:24:in `_app_views_request__incoming_correspondence_html_erb___4053020488255440338_85045320'
 app/views/request/_correspondence.html.erb:4:in `_app_views_request__correspondence_html_erb__2668726388495238954_86949000'
 app/views/request/show.html.erb:68:in `block in _app_views_request_show_html_erb___283401135198515593_88463540'
 app/views/request/show.html.erb:66:in `_app_views_request_show_html_erb___283401135198515593_88463540'
 app/controllers/request_controller.rb:133:in `block (3 levels) in show'
 app/controllers/request_controller.rb:132:in `block in show'
 lib/alaveteli_localization.rb:43:in `with_locale'
 app/controllers/request_controller.rb:89:in `show'
 app/controllers/application_controller.rb:120:in `record_memory'
 lib/strip_empty_sessions.rb:13:in `call'
