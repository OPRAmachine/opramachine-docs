+++
# Type of content, set "slide" to display it fullscreen with reveal.js
type="page"
title = "Statistics Page Broken"
description = "The statistics page is broken"
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

The statistics page is currently broken. We are investigating the cause of the problem

## Github issue (Upstream)

https://github.com/mysociety/alaveteli/issues/4433

## Raw text of error message

A Math::DomainError occurred in statistics#index:

 Numerical argument is out of domain - "sqrt"
 lib/confidence_intervals.rb:28:in `sqrt'


-------------------------------
Request:
-------------------------------

 * URL        : https://opramachine.com/statistics
 * HTTP Method: GET
 * IP address : 54.161.187.202
 * Parameters : {"controller"=>"statistics", "action"=>"index"}
 * Timestamp  : 2017-12-20 21:57:55 -0500
 * Server : opramachine.com
 * Rails root : /var/www/opramachine.com/alaveteli
 * Process: 23591

-------------------------------
Session:
-------------------------------

 * session id: [FILTERED]
 * data: {"session_id"=>"95647a59eaf52bc425f666123ae9fff8", "locale"=>"en"}

-------------------------------
Environment:
-------------------------------

 * GATEWAY_INTERFACE                              : CGI/1.2
 * HTTP_ACCEPT                                    : */*
 * HTTP_ACCEPT_ENCODING                           : gzip,deflate
 * HTTP_CONNECTION                                : close
 * HTTP_HOST                                      : opramachine.com
 * HTTP_RANGE                                     : bytes=0-16384
 * HTTP_USER_AGENT                                : Slackbot-LinkExpanding 1.0 (+https://api.slack.com/robots)
 * HTTP_VERSION                                   : HTTP/1.0
 * HTTP_X_ACCEL_MAPPING                           : /var/www/opramachine.com/alaveteli/cache/zips/production/download=/download
 * HTTP_X_FORWARDED_FOR                           : 54.161.187.202
 * HTTP_X_FORWARDED_PROTO                         : https
 * HTTP_X_REAL_IP                                 : 54.161.187.202
 * HTTP_X_SENDFILE_TYPE                           : X-Accel-Redirect
 * ORIGINAL_FULLPATH                              : /statistics
 * ORIGINAL_SCRIPT_NAME                           :
 * PATH_INFO                                      : /statistics
 * QUERY_STRING                                   :
 * REMOTE_ADDR                                    : 127.0.0.1
 * REQUEST_METHOD                                 : GET
 * REQUEST_PATH                                   : /statistics
 * REQUEST_URI                                    : /statistics
 * ROUTES_53640860_SCRIPT_NAME                    :
 * SCRIPT_NAME                                    :
 * SERVER_NAME                                    : opramachine.com
 * SERVER_PORT                                    : 80
 * SERVER_PROTOCOL                                : HTTP/1.1
 * SERVER_SOFTWARE                                : thin 1.5.1 codename Straight Razor
 * action_controller.instance                     : #<StatisticsController:0x0000001129a7a0>
 * action_dispatch.backtrace_cleaner              : #<Rails::BacktraceCleaner:0x0000000a89b570>
 * action_dispatch.cookies                        : #<ActionDispatch::Cookies::CookieJar:0x0000000d69b9e8>
 * action_dispatch.cookies_digest                 :
 * action_dispatch.cookies_serializer             : hybrid
 * action_dispatch.encrypted_cookie_salt          : encrypted cookie
 * action_dispatch.encrypted_signed_cookie_salt   : signed encrypted cookie
 * action_dispatch.http_auth_salt                 : http authentication
 * action_dispatch.key_generator                  : #<ActiveSupport::CachingKeyGenerator:0x000000095c7368>
 * action_dispatch.logger                         : #<ActiveSupport::Logger:0x0000000655fa18>
 * action_dispatch.parameter_filter               : [:password]
 * action_dispatch.redirect_filter                : []
 * action_dispatch.remote_ip                      : 54.161.187.202
 * action_dispatch.request.accepts                : [#<Mime::Type:0x00000011298f68 @synonyms=[], @symbol=nil, @string="*/*", @hash=4306184708532017714>]
 * action_dispatch.request.content_type           :
 * action_dispatch.request.formats                : [#<Mime::Type:0x00000011298f68 @synonyms=[], @symbol=nil, @string="*/*", @hash=4306184708532017714>]
 * action_dispatch.request.parameters             : {"controller"=>"statistics", "action"=>"index"}
 * action_dispatch.request.path_parameters        : {:controller=>"statistics", :action=>"index"}
 * action_dispatch.request.query_parameters       : {}
 * action_dispatch.request.request_parameters     : {}
 * action_dispatch.request.unsigned_session_cookie: {"session_id"=>"95647a59eaf52bc425f666123ae9fff8"}
 * action_dispatch.request_id                     : 7b0d26e2-9544-49b8-a094-c9861a3e1076
 * action_dispatch.routes                         : #<ActionDispatch::Routing::RouteSet:0x0000000664fd38>
 * action_dispatch.secret_key_base                : this default is insecure as code is open source, please override for live sites in config/general; this will do for local development
 * action_dispatch.secret_token                   :
 * action_dispatch.show_detailed_exceptions       : false
 * action_dispatch.show_exceptions                : true
 * action_dispatch.signed_cookie_salt             : signed cookie
 * async.callback                                 : #<Method: Thin::Connection#post_process>
 * async.close                                    : #<EventMachine::DefaultDeferrable:0x0000000f5e4480>
 * newrelic.transaction_started                   : true
 * rack.errors                                    : #<IO:0x00000002041b98>
 * rack.input                                     : #<StringIO:0x0000000f5e4ca0>
 * rack.multiprocess                              : false
 * rack.multithread                               : false
 * rack.request.cookie_hash                       : {}
 * rack.request.query_hash                        : {}
 * rack.request.query_string                      :
 * rack.run_once                                  : false
 * rack.session                                   : #<ActionDispatch::Request::Session:0x0000000f6343b8>
 * rack.session.options                           : #<ActionDispatch::Request::Session::Options:0x0000000f634368>
 * rack.url_scheme                                : http
 * rack.version                                   : [1, 0]

-------------------------------
Backtrace:
-------------------------------

 lib/confidence_intervals.rb:28:in `sqrt'
 lib/confidence_intervals.rb:28:in `ci_bounds'
 app/models/public_body.rb:722:in `block in get_request_percentages'
 app/models/public_body.rb:721:in `each'
 app/models/public_body.rb:721:in `each_with_index'
 app/models/public_body.rb:721:in `each'
 app/models/public_body.rb:721:in `map'
 app/models/public_body.rb:721:in `get_request_percentages'
 app/models/statistics.rb:49:in `block (2 levels) in public_bodies'
 app/models/statistics.rb:43:in `each'
 app/models/statistics.rb:43:in `block in public_bodies'
 app/models/statistics.rb:42:in `each'
 app/models/statistics.rb:42:in `public_bodies'
 app/controllers/statistics_controller.rb:7:in `index'
 app/controllers/application_controller.rb:120:in `record_memory'
 lib/strip_empty_sessions.rb:13:in `call'
