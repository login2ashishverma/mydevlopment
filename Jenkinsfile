node {
	stage 'Checkout'
		checkout scm

	stage 'Build'
		bat 'nuget restore SampleAppCICD.sln'
		bat "\"${tool 'MSBuild'}\" SampleAppCICD.sln /p:Configuration=Release /p:Platform=\"Any CPU\" /p:ProductVersion=1.0.0.${env.BUILD_NUMBER}"

	stage 'Archive'
		archive 'SampleAppCICD/bin/Release/**'

}
