

node {
	stage('PrintAll') {
		echo "BRANCH_NAME: ${env.BRANCH_NAME}"
		echo "CHANGE_ID: ${env.CHANGE_ID}"
		echo "CHANGE_URL: ${env.CHANGE_URL}"
		echo "CHANGE_TITLE: ${env.CHANGE_TITLE}"
		echo "CHANGE_TITLE: ${env.CHANGE_AUTHOR}"
		echo "CHANGE_AUTHOR_DISPLAY_NAME: ${env.CHANGE_AUTHOR_DISPLAY_NAME}"
		echo "CHANGE_AUTHOR_EMAIL: ${env.CHANGE_AUTHOR_EMAIL}"
		echo "CHANGE_TARGET: ${env.CHANGE_TARGET}"
		echo "CHANGE_BRANCH: ${env.CHANGE_BRANCH}"
		echo "CHANGE_FORK: ${env.CHANGE_FORK}"
		echo "BUILD_NUMBER: ${env.BUILD_NUMBER}"
		echo "BUILD_URL: ${env.BUILD_URL}"

		commitInfo = sh (
		      script: 'git --no-pager show -s --format=\'%h|%an|%ae|%s\'',
		      returnStdout: true
		).trim()
		echo "Commit Info: ${commitInfo}"
	}
}
