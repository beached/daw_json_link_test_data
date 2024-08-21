# Copyright (c) Darrell Wright
#
# Distributed under the Boost Software License, Version 1.0. (See accompanying
# file LICENSE or copy at http://www.boost.org/LICENSE_1_0.txt)
#
# Official repository: https://github.com/beached/daw_json_link_test_data
#

cmake_minimum_required(VERSION 3.14)

project("daw-json-link-test-data"
        VERSION "1.0.0"
				DESCRIPTION "Data used by JSON Link for testing"
        HOMEPAGE_URL "https://github.com/beached/daw_json_link_test_data"
        )

				file( GLOB JSON_FILES "${PROJECT_SOURCE_DIR}\*.json" )
				file( COPY ${JSON_FILES} DESTINATION td )
