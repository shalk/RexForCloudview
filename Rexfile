user "shalk";
password "shuqi";
pass_auth;

group myservers => "localhost";

desc "Get Disk Free";
task "disk_free",sub {
    my $output = run " df -h ";
    say $output;
};

desc "Process Information";
task "ps_info",sub {
    my $output = run "ps ";
    say $output;
    Rex::Logger::info "Green Message";
    Rex::Logger::info "Yellow Message","warn";
    Rex::Logger::info "Red ,Message","error";
}
