pipeline{
agent any;
stages{
stage ('build'){
steps{
echo "this is build stage"
sh 'sleep 5'
}
}
stage ('test parallel'){
parallel{
steps{
echo "this is parallel stage"
sh 'sleep 5'
}
}
}
}
}
