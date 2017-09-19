CMAKE_MINIMUM_REQUIRED(VERSION 3.0.2)
set(WORKSPACE_DIR ${CMAKE_SOURCE_DIR}/../.. CACHE PATH "root of the packages workspace directory")
list(APPEND CMAKE_MODULE_PATH ${WORKSPACE_DIR}/share/cmake/system) # using generic scripts/modules of the workspace
include(Package_Definition NO_POLICY_SCOPE)

PROJECT(cdd)

declare_PID_Package(	
	AUTHOR 		vsamy
	INSTITUTION LIRMM
	MAIL 		vincent.samy@lirmm.fr
	 ADDRESS git@github.com:vsamy/cdd.git
	 YEAR 		2017 
	LICENSE 	CeCILL-C
	DESCRIPTION "This is a polytope library. Forked from Fukuda's library: https://www.inf.ethz.ch/personal/fukudak/cdd_home/"
)

set_PID_Package_Version(0 95 0)

#now finding packages

build_PID_Package()

